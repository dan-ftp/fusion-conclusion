---
layout: page
title: "Subscribe"
permalink: /subscribe/
---

<form
  id="bd-form"
  action="https://buttondown.com/api/emails/embed-subscribe/fusionconclusion"
  method="post"
  target="bd-hidden-iframe"
  class="embeddable-buttondown-form"
>
  <input type="email" name="email" id="bd-email" autocomplete="email" required />
  <input type="hidden" name="embed" value="1" />
  <!-- optional -->
  <input type="hidden" name="tag" value="website" />

  <button id="bd-button" type="submit">Subscribe</button>

  <div id="bd-status" aria-live="polite" style="margin-top:0.75rem; display:none;"></div>
</form>

<iframe
  id="bd-hidden-iframe"
  name="bd-hidden-iframe"
  style="display:none"
></iframe>

<script>
(() => {
  const form = document.getElementById("bd-form");
  const btn = document.getElementById("bd-button");
  const emailInput = document.getElementById("bd-email");
  const status = document.getElementById("bd-status");
  const iframe = document.getElementById("bd-hidden-iframe");

  let pending = false;
  let originalText = btn.textContent;
  let watchdog = null;

  function showStatus(text) {
    status.style.display = "block";
    status.textContent = text;
  }

  form.addEventListener("submit", () => {
    // Save original label once (yours currently says "SUBSCRIBE AS ...")
    if (!btn.dataset.originalText) btn.dataset.originalText = btn.textContent;
    originalText = btn.dataset.originalText;

    pending = true;
    btn.disabled = true;
    btn.textContent = "Subscribing…";

    const email = (emailInput?.value || "").trim();
    showStatus(email
      ? `Submitted ${email}. Check your inbox for a confirmation email.`
      : "Submitted. Check your inbox for a confirmation email."
    );

    // If the iframe never loads (blocked/network), give the user a helpful nudge.
    clearTimeout(watchdog);
    watchdog = setTimeout(() => {
      if (!pending) return;
      btn.disabled = false;
      btn.textContent = originalText;
      showStatus("Hmm — that didn’t finish. Please try again, or use the direct subscribe link.");
      pending = false;
    }, 12000);
  });

  // Fires when Buttondown returns a response into the hidden iframe
  iframe.addEventListener("load", () => {
    if (!pending) return;
    pending = false;
    clearTimeout(watchdog);

    btn.textContent = "Subscribed ✓";
    showStatus("Success — confirmation email sent. Please click the link in that email to finish.");

    // Optional: re-enable later (in case they typed the wrong email)
    setTimeout(() => {
      btn.disabled = false;
      btn.textContent = originalText;
    }, 15000);
  });
})();
</script>
