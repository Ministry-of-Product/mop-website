---
layout: default
title: Ministry of Product
description: A venture studio that builds its own products, and an advisory practice that helps founder-led teams build theirs.
meta_description: Ministry of Product — a venture studio that builds and incubates its own products, and an advisory practice for founder-led teams in Seattle.
numbered_sections: true
---

<div class="workshop-hero">
  <div class="gearstack" aria-hidden="true">
    <span class="g g1 spin"></span>
    <span class="g g2 spin-rev"></span>
  </div>
  <div class="hero-content">
    <span class="eyebrow">Venture Studio · Advisory</span>
    <h1>Ministry of <span class="em">Product</span></h1>
    <p class="sub">We turn ideas into real, profitable businesses — building products of our own, and helping founder-led teams build theirs.</p>
    <div class="cta">
      <a class="btn btn-copper" href="/venture-studio/">Explore the Venture Studio <span class="gear spin" style="font-size:15px"></span></a>
      <a class="btn btn-ghost" href="/advisory/">Work with us →</a>
    </div>
  </div>
</div>


- **The Venture Studio** identifies opportunities, builds products, runs experiments, and incubates businesses of our own.
- **Advisory & Consulting** helps founder-led teams make better product, AI, and operational decisions — and builds the software when it's the right move.
- **Innovation Commons** where anyone can work on an idea.


<div class="mop-stats">
  <div class="stat"><span class="num" id="stat-fragments">336</span><span class="lbl">Ideas<br>explored</span></div>
  <div class="stat"><span class="num" id="stat-ventures">14</span><span class="lbl">Ventures<br>taking shape</span></div>
  <div class="stat"><span class="num">20</span><span class="lbl">Years<br>of craft</span></div>
</div>
<script>
(function () {
  var FLOOR_FRAGMENTS = 50;
  var FLOOR_VENTURES  = 10;
  var elF = document.getElementById('stat-fragments');
  var elV = document.getElementById('stat-ventures');
  fetch('https://idea-growth-backend-mop-j6pdv7rpoq-uc.a.run.app/api/stats/public')
    .then(function (r) { return r.json(); })
    .then(function (data) {
      if (elF && typeof data.fragments === 'number' && data.fragments >= FLOOR_FRAGMENTS) {
        elF.textContent = data.fragments.toLocaleString();
      }
      if (elV && typeof data.ventures === 'number' && data.ventures >= FLOOR_VENTURES) {
        elV.textContent = data.ventures.toLocaleString();
      }
    })
    .catch(function () { /* network failure — static fallback values remain */ });
}());
</script>

---

## Venture Studio

We build, launch, and incubate our own products and businesses. Ideas become prototypes, prototypes earn users, and the ones that prove real spin out as companies.

That work runs on an [Innovation Commons](/innovation-commons/) — an invite-only practice where builders explore ideas before they become companies, and ownership is earned through contribution rather than assigned upfront. It's the engine that turns ideas into ventures.

<div style="display: flex; flex-wrap: wrap; gap: 0.75rem; align-items: center; margin: 1.5rem 0;">
  <a class="btn btn-copper" href="/venture-studio/">Explore the Venture Studio →</a>
  <a class="btn btn-ghost" href="/venturestudio/">Run the simulator →</a>
</div>

---

## Advisory & Consulting

We partner with founders and executives to turn vision into working software — using AI-native development to move faster than a traditional team could on its own. We bring the same judgment we develop building our own ventures: what matters now, what can wait, and where effort will compound versus stall.

**Build** — Embed as a product partner on new software ideas, from concept to live product. Product strategy, architecture decisions, and execution — so founders stay focused on the business.

**Advise** — For teams with existing engineers, fractional CPO or product lead: setting direction with OKRs, shaping roadmap, keeping the team building the right things in the right order.

**Accelerate** — Integrate AI tooling into your development process to cut the time and cost of building, testing, and iterating.

[Work with us →](/advisory/)

## Ventures

A few of the ventures we've built and launched:

<div class="mop-plates">

  <div class="mop-plate trueup">
    <a class="plate-link" href="/ventures/trueup/" aria-label="View the TrueUp venture"></a>
    <h3>TrueUp</h3>
    <div class="tl">Expert guidance over video</div>
    <p>Remote expert guidance for skilled tradespeople. Video calls with AI-generated summaries, on-screen annotations, and automatic recording. Experts get paid for their knowledge; clients get professional documentation of every session.</p>
    <a class="more" href="/ventures/trueup/">View the venture →</a>
  </div>

  <div class="mop-plate sound">
    <a class="plate-link" href="/ventures/soundpoints/" aria-label="View the SoundPoints venture"></a>
    <h3>SoundPoints</h3>
    <div class="tl">Discover the world through sound</div>
    <p>Location-based audio experiences. Creators pin content to GPS coordinates; explorers unlock it by being there. Built for walking tours, podcast extensions, and site-specific audio art. Currently in beta.</p>
    <a class="more" href="/ventures/soundpoints/">View the venture →</a>
  </div>

  <div class="mop-plate fortunate">
    <a class="plate-link" href="/ventures/fortunatematch/" aria-label="View the FortunateMatch venture"></a>
    <h3>FortunateMatch</h3>
    <div class="tl">Connections at every event</div>
    <p>AI-powered event matchmaking. Attendees declare what they need and what they offer; the system surfaces the highest-value introductions in real time. Built for organizers who want networking that produces real outcomes.</p>
    <a class="more" href="/ventures/fortunatematch/">View the venture →</a>
  </div>

</div>

---

[Explore the Venture Studio →](/venture-studio/) [Work with us →](/advisory) [About →](/about)
{: .cta-row}
