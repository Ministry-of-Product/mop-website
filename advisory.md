---
layout: default
title: Working Together
description: Convert fit into conversations while filtering aggressively. For experienced operators with revenue, clients, and authority.
permalink: /advisory/
meta_description: Work with Ministry of Product to scale your business with AI-enabled systems. For experienced operators with revenue, clients, and authority.
---

# Working Together

Convert fit into conversations while filtering aggressively.

## Who This Is For

- **Businesses with existing revenue, clients, and authority**
- Founders or operators trying to scale strategy, insight, or operations with AI
- Teams overwhelmed by possibilities rather than blocked by capability
- People ready to make decisions, not just explore possibilities

## Who This Is Not For

- Idea-only founders without revenue or clients
- People afraid of ideas being "stolen"
- Vendor shoppers or tire-kickers
- Teams without budget or decision-making authority
- People looking for free work, demos, or speculative effort

If you're in the second group, this isn't the right fit. That's intentional.

## What We'll Do

We start with a conversation about your situation, what you've tried, and where you're stuck. From there, we identify:

1. **The decision that matters** — What actually needs to be decided right now?
2. **The experiment** — What's the smallest thing we can build to test this?
3. **Success criteria** — How will we know if this is working?
4. **Next steps** — What happens after this experiment?

No long-term commitments. No vendor pitches. Just clarity about what to do next.

## What to Expect

- **Decision leadership** — Help identifying what to build, in what order
- **Implementation credibility** — Actually building experiments, not just frameworks
- **Clear boundaries** — We'll say no to things that don't make sense
- **Experiments over commitments** — Early systems are tests, not permanent infrastructure

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

