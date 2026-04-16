---
layout: default
title: Working Together
description: I partner with founders and executives to build software products—from first conversation to live product.
permalink: /advisory/
meta_description: Work with Ministry of Product — embedded product partner for founders and executives building software.
---

# Working Together

## How I can help

I work with founders and executives at three levels, depending on where you are and what you need.

**Build** — You have an idea and want it to become real software. I embed as a product partner: shaping the concept, making technical decisions, and driving execution. You stay focused on the business; I make sure the right thing gets built and shipped. This is the fastest path from vision to something in market.

**Advise** — You already have a team building. I come in as a fractional CPO or product lead: setting direction with OKRs, making roadmap decisions, and keeping execution connected to strategy. Useful when the engineering is there but product leadership isn’t.

**Accelerate** — You want to move faster and spend less building what you already know needs to exist. I bring AI-native development practices into your process — not as a novelty, but as genuine leverage on the time and cost of building, testing, and iterating.

## How an engagement starts

Most engagements begin with a conversation about what you’re trying to build and why. From there, the shape of the work becomes clear quickly — sometimes it’s a short sprint to validate an idea, sometimes it’s an ongoing partnership.

I don’t take on many projects at once. When I’m in, I’m genuinely in.

## Who this works best for

Founders and executives with a real idea and real stakes. People who value judgment over activity, and who want a partner who can both think through the hard questions and make things real. Engagements work best when there’s clear ownership, honest feedback, and space to learn from what gets built.

## If this sounds like the right fit

[Contact me](/advisory#contact) and tell me what you’re working on.

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
