---
layout: page
title: "Subscribe"
permalink: /subscribe/
---

<form
  id="bd-form"
  action="https://buttondown.com/api/emails/embed-subscribe/fusionconclusion"
  method="post"
  target="bd-response"
  class="embeddable-buttondown-form"
>
  <label for="bd-email">Email</label>
  <input
    id="bd-email"
    type="email"
    name="email"
    placeholder="you@example.com"
    autocomplete="email"
    inputmode="email"
    required
  />

  <!-- Required for the embeddable form endpoint -->
  <input type="hidden" name="embed" value="1" />

  <!-- Optional: auto-tag subscribers -->
  <input type="hidden" name="tag" value="website" />

  <!-- Optional: UTM params (Buttondown supports these in the form body) -->
  <input type="hidden" name="utm_source" value="fusionconclusion.com" />
  <input type="hidden" name="utm_medium" value="web" />
  <input type="hidden" name="utm_campaign" value="subscribe_form" />

  <button id="bd-submit" type="submit">Subscribe</button>

  <!-- Friendly status line (truthful; doesn't claim success) -->
  <p id="bd-status" role="status" aria-live="polite" style="margin: 0.75rem 0 0; display:none;"></p>

  <!-- This iframe will display Buttondown's real response (accurate: success vs blocked) -->
  <iframe
    id="bd-response"
    name="bd-response"
    title="Subscription status"
    style="display:none; width:100%; height:160px; border:1px solid rgba(0,0,0,0.15); border-radius:8px; margin-top:0.75rem;"
  ></iframe>

  <p style="margin: 0.75rem 0 0;">
    Prefer a hosted form?
    <a
      href="https://buttondown.com/fusionconclusion"
      target="_blank"
      rel="noopener"
    >Subscribe on Buttondown</a>
  </p>
</form>

<script>
(() => {
  const form = document.getElementById("bd-form");
  const email = document.getElementById("bd-email");
  const btn = document.getElementById("bd-submit");
  const status = document.getElementById("bd-status");
  const iframe = document.getElementById("bd-response");

  const baseBtnText = btn.textContent;
  let pending = false;
  let watchdog = null;

  function setStatus(text) {
    status.style.display = "block";
    status.textContent = text;
  }

  function updateButtonText() {
    if (pending) return;
    const v = (email.value || "").trim();
    btn.textContent = v ? `Subscribe as ${v}` : baseBtnText;
  }

  email.addEventListener("input", updateButtonText);
  updateButtonText();

  form.addEventListener("submit", (e) => {
    // Keep browser validation bubbles working:
    if (!form.reportValidity()) {
      e.preventDefault();
      return;
    }

    pending = true;
    btn.disabled = true;
    btn.textContent = "Submitting…";

    // Show truthful, positive messaging
    setStatus("Submitting… If accepted, you’ll receive a confirmation email shortly. See the status message below.");

    // Show the iframe so the user sees Buttondown’s actual response (success OR blocked)
    iframe.style.display = "block";

    // If the iframe never finishes (blocked by CSP/network), recover gracefully
    clearTimeout(watchdog);
    watchdog = setTimeout(() => {
      if (!pending) return;
      pending = false;
      btn.disabled = false;
      updateButtonText();
      setStatus("That didn’t finish loading. Please try again, or use the hosted subscribe link below.");
      // Keep iframe visible in case it loads late
    }, 12000);
  });

  // Fires when Buttondown returns its response into the iframe
  iframe.addEventListener("load", () => {
    if (!pending) return;
    pending = false;
    clearTimeout(watchdog);

    btn.textContent = "Submitted ✓";
    setStatus("Done — please read the status in the box below. (If you’re asked to confirm, check your inbox.)");

    // Re-enable after a moment in case they typed the wrong email
    setTimeout(() => {
      btn.disabled = false;
      updateButtonText();
    }, 8000);
  });
})();
</script>
