---
layout: default
title: Working Together
description: Convert fit into conversations while filtering aggressively. For experienced operators with revenue, clients, and authority.
permalink: /advisory/
meta_description: Work with Ministry of Product to scale your business with AI-enabled systems. For experienced operators with revenue, clients, and authority.
---

# Working Together

## How I can help

I support business owners by helping ideas move from vague curiosity to something you can actually react to.
This work is collaborative, flexible, and shaped by how your business really operates.

## Thinking together

We spend time understanding:
- where work feels heavier than it should
- which parts of the business absorb too much attention
- what tends to break down when things get busy or change

These conversations are often clarifying on their own.

## Trying small experiments

From there, we choose one small thing to explore.
That might look like:
- me building a rough version of an idea so you can see it
- you experimenting with an AI tool and sharing what stood out
- using a simple app generator as a shared sketchpad

The goal is to make ideas visible quickly, so we can learn from them.

## Handling the “doing”

Early on, I often take care of the setup, building, or experimentation so you don’t have to pause your business to learn new tools.
If you later want to bring that work inside your team, we plan a thoughtful handoff that keeps everything understandable and usable.

## Staying flexible

Some people come for a single experiment.
Others enjoy an ongoing rhythm of conversations and small iterations.
There’s no fixed path. We let usefulness guide the work.

## If this sounds useful

[Contact me](/advisory#contact) to discuss your situation.

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
