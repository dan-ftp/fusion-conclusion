---
layout: page
title: "Subscribe"
permalink: /subscribe/
---

<form
  action="https://buttondown.com/api/emails/embed-subscribe/fusionconclusion"
  method="post"
  class="embeddable-buttondown-form"
>
  <label for="bd-email">Email</label>
  <input
    id="bd-email"
    type="email"
    name="email"
    placeholder="you@example.com"
    autocomplete="email"
    required
  />

  <input type="hidden" name="embed" value="1" />
  <input type="hidden" name="tag" value="website" />

  <!-- Optional: tracking -->
  <input type="hidden" name="utm_source" value="fusionconclusion.com" />
  <input type="hidden" name="utm_medium" value="web" />
  <input type="hidden" name="utm_campaign" value="subscribe_form" />

  <button type="submit">Subscribe</button>

  <p style="margin-top:0.75rem;">
    Trouble with the form?
    <a href="https://buttondown.com/fusionconclusion" target="_blank" rel="noopener">
      Subscribe here
    </a>
  </p>
</form>

