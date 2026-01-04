---
layout: page
title: "Subscribe"
permalink: /subscribe/
---

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

  function showStatus(html) {
    status.style.display = "block";
    status.innerHTML = html;
  }

  form.addEventListener("submit", () => {
    if (!btn.dataset.originalText) btn.dataset.originalText = btn.textContent;
    originalText = btn.dataset.originalText;

    pending = true;
    btn.disabled = true;
    btn.textContent = "Submitting…";

    const email = (emailInput?.value || "").trim();

    showStatus(`
      <strong>Submitted.</strong>
      ${email ? ` (${email})` : ``}
      <br/>
      If your address is accepted, you’ll receive a confirmation email shortly.
      <br/>
      If you don’t receive anything, try the hosted subscribe page:
      <a href="https://buttondown.com/fusionconclusion" target="_blank" rel="noopener">Subscribe here</a>.
    `);

    clearTimeout(watchdog);
    watchdog = setTimeout(() => {
      if (!pending) return;
      pending = false;
      btn.disabled = false;
      btn.textContent = originalText;
      showStatus(`
        <strong>Hmm — didn’t finish.</strong><br/>
        Please try again, or use the hosted subscribe page:
        <a href="https://buttondown.com/fusionconclusion" target="_blank" rel="noopener">Subscribe here</a>.
      `);
    }, 12000);
  });

  iframe.addEventListener("load", () => {
    if (!pending) return;
    pending = false;
    clearTimeout(watchdog);

    // IMPORTANT: don't claim success — we can't know if it was blocked.
    btn.textContent = "Submitted ✓";
    showStatus(status.innerHTML); // keep the honest message above

    setTimeout(() => {
      btn.disabled = false;
      btn.textContent = originalText;
    }, 15000);
  });
})();
</script>
