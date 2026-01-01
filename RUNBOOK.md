
# FusionConclusion.com — Post-cutover Runbook

## Primary URLs
- Canonical: https://www.fusionconclusion.com/
- Apex redirect: https://fusionconclusion.com/ → https://www.fusionconclusion.com/

## Quick site health checks
```bash
# www should be 200
curl -sSIL https://www.fusionconclusion.com/ | sed -n '1,15p'

# apex should be 301 to www
curl -sSIL https://fusionconclusion.com/ | sed -n '1,15p'

# key endpoints
base="https://www.fusionconclusion.com"
for p in "robots.txt" "sitemap.xml" "feed.xml" "rss/"; do
  echo "-- $p --"
  curl -sSIL "${base}/${p}?nocache=$(date +%s)" | sed -n '1,12p'
done

