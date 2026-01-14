---
layout: default
title: Advisory & Guidance
description: Direct help making better next-step decisions for your AI product or prototype.
permalink: /advisory/
meta_description: Get direct help making better next-step decisions for your AI product. For builders who have built something and are now directionally stuck.
---

# Advisory & Guidance

This is for builders who have already built something and are now directionally stuck.

## Who This Is For

- You've built a working prototype or product with AI
- You're technically capable but uncertain about what to do next
- You're asking "I've built this... now what?"
- You need judgment about sequencing, not more features

This is not for beginners or enterprise committees. It's for solo builders, product-minded engineers, and early founders who need clarity.

## What Problems This Solves

- **Sequencing decisions** — What matters now vs. later
- **Feature vs. product vs. company** — Understanding what you actually have
- **Narrowing vs. expanding** — When to focus and when to explore
- **Moving into reality** — Getting ideas into contact with actual users faster
- **Avoiding waste** — Not spending months on the wrong next step

## How It Works

We start with a conversation about what you've built and where you're stuck. From there, we identify the decision that actually matters and what should happen next.

No hard sell. No long-term commitments. Just clarity about your specific situation.

## Get Started

[Contact me](/advisory#contact) to discuss your situation. We'll determine if there's a fit and how to proceed.

---

## Contact

<div id="contact"></div>
<button id="contactBtn" class="cta-button">Start a Conversation</button>

<!-- Contact Modal -->
<div id="contactModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    <iframe 
      id="googleFormIframe"
      src="https://docs.google.com/forms/d/e/1FAIpQLSeoBMkQfFJiFgrceWSoldQSoLvsBLEReSWRbpQ-Hg_t3qjFXw/viewform?embedded=true" 
      width="640" 
      height="836" 
      frameborder="0" 
      marginheight="0" 
      marginwidth="0"
      allow="fullscreen"
      loading="lazy"
      referrerpolicy="no-referrer-when-downgrade"
      title="Contact the Ministry of Product">
      Loading…
    </iframe>
  </div>
</div>

<script>
// Suppress harmless Google Forms font loading errors
(function() {
  const originalError = console.error;
  const originalWarn = console.warn;
  
  console.error = function(...args) {
    const message = args.join(' ');
    if (message.includes('docs.google.com') && 
        (message.includes('fonts') || 
         message.includes('woff2') || 
         message.includes('ERR_FILE_NOT_FOUND') ||
         message.includes('filesystem:'))) {
      return;
    }
    originalError.apply(console, args);
  };
  
  window.addEventListener('unhandledrejection', function(e) {
    const reason = e.reason ? String(e.reason) : '';
    if (reason.includes('docs.google.com') && reason.includes('fonts')) {
      e.preventDefault();
    }
  });
})();

// Modal functionality
document.addEventListener('DOMContentLoaded', function() {
  const modal = document.getElementById('contactModal');
  const btn = document.getElementById('contactBtn');
  const span = document.getElementsByClassName('close')[0];

  if (btn) {
    btn.onclick = function() {
      modal.style.display = 'block';
    }
  }

  if (span) {
    span.onclick = function() {
      modal.style.display = 'none';
    }
  }

  window.onclick = function(event) {
    if (event.target == modal) {
      modal.style.display = 'none';
    }
  }
});
</script>

