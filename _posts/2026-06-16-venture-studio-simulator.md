---
layout: default
title: "The Venture Studio Simulator: Watch a Fund Become Companies"
date: 2026-06-16
categories: venture-studio
excerpt: "Every time I explain how the Ministry of Product venture studio works, I reach for a slide full of arrows and watch people nod without really seeing it. So I built a version you can run — press Advance One Month and watch the money move, the ownership fill in, and companies spin out."
---

# The Venture Studio Simulator: Watch a Fund Become Companies

Every time I try to explain how the Ministry of Product venture studio works, I end up at a whiteboard drawing arrows. Investors fund the studio, the studio builds companies, the winners spin out. People nod. But nobody ever actually *sees* the money move, the ownership fill in, or the funnel thin out — and that's the part that makes it make sense.

So I built a version you can run. It's a single web page: press **Advance One Month** and watch the whole machine turn.

**[Open the Venture Studio Simulator →](/venturestudio/)**

<p style="border-left:3px solid #6366f1;padding-left:1rem;color:#475569;">
This is an explanatory model, not a legal cap table. Every ownership, revenue, and distribution number in it is <b>simulated, estimated, and illustrative</b>. The point is to make the flow understandable, not to be financially exact.
</p>

## What it's modeling

A venture studio is an operating company that builds startups itself — generating ideas, staffing them, launching them, and spinning out the ones that work as their own companies. Investors back a whole **cohort** of that work rather than a single bet, so what they're buying is exposure to a portfolio, not a lottery ticket.

The simulator rests on three real pieces of how we run things:

- **The cohort fund — "VSC1" (Venture Studio Cohort 1).** A pool of investor capital with a raise target (default **$300,000**) that funds one year of venture creation.
- **The product pathway.** Every venture climbs ten release levels, from **RL1 Idea** to **RL10 Stable**. Each level is a milestone, not a calendar date.
- **BSSS — "Big Slice / Small Slice."** The ownership model we use in the [Innovation Commons](/innovation-commons): ownership is *earned* as the work happens, not handed out up front.

## The cast

**Investors** commit cash to the fund. Set the raise target, fill the fund, add investors, and each one gets a *cohort share* — their contribution divided by the total raise. Put in $150k of a $300k raise and you own half the cohort.

**Participants** do the work and earn the ownership. They come in two kinds that behave the same way but get accounted for separately: **contributors** are the builders — engineering, product, marketing — and their funding is a capital cost; **operations** is the studio overhead, Ministry of Product itself running the machine, and its funding is an operational cost.

Every participant earns a share of each venture through work, and every participant can draw monthly cash from the fund. What they give up for that cash is where it gets interesting.

## How ownership is earned: BSSS

A **Big Slice** is a fixed chunk of a venture's ownership attached to a milestone. Each of the ten stages opens one, and they add to 100%:

| Stage | Name | Big Slice |
|------|------|----------:|
| RL1 | Idea | 4% |
| RL2 | Vision | 4% |
| RL3 | Prototype | 4% |
| RL4 | Play Test | 12% |
| RL5 | Release | 16% |
| RL6 | Users | 12% |
| RL7 | Audience | 12% |
| RL8 | Monetized | 12% |
| RL9 | Scalable | 12% |
| RL10 | Stable | 12% |

A **Small Slice** is what a contributor earns *inside* a Big Slice, proportional to the work they put in: `(your points ÷ total points in the slice) × Big Slice %`. Completed slices lock — once a stage is done, the ownership earned in it can't be diluted later. Future stages stay unallocated until the work actually happens, which is why a young venture's ownership donut is mostly grey. Ownership fills in as the venture climbs.

## The part most cap-table diagrams skip: investors *buy* their equity

The participants earn 100% of every venture through their work. Investors end up owning a piece only because participants *sell* it to them — and the currency is the fund.

Each participant has two dials: **Funded $/mo**, the cash they draw each month, and **Gives up %**, the cut of their earned shares they hand to the investor pool in exchange for it.

Take the default operations entity, Ministry of Product: it earns a **35%** BSSS share, draws **$15,000/month**, and gives up **35%** of what it earns. So it keeps `35% × (1 − 0.35) = 22.75%`, and the investors buy `35% × 0.35 = 12.25%`. That 12.25% then splits among the individual investors by their cohort share.

A participant who takes no money keeps everything they earn, and the investors get nothing from them. Which is the whole economic model in one line:

> **Take the fund's cash, give up equity. Bootstrap, keep your equity.**

Because the investors only own what people sold them, the fund drains only when someone actually draws. If nobody takes money this month, the tank holds. Press Advance and you'll watch it drop by exactly what was drawn, with a little "−$15,000" floating off the top.

## The monthly machine

**Advance One Month** is the heart of it. Each month the fund pays out what participants draw and the tank drains; a new idea might enter the pipeline; ventures advance a stage, stall, or get **killed**; BSSS slices fill; survivors grow customers and revenue; and everything gets re-checked for spinout eligibility.

The pipeline shows this as a funnel — wide on the left where ideas enter, narrowing to the right as they're selected or killed. It's a funnel on purpose, not three tidy bets. Most ideas are supposed to fail, and killing the weak ones early is how the studio concentrates its attention.

## Spinouts

A venture earns its way out into its own company when it clears five bars — **MRR ≥ $5,000**, positive cash flow, repeatable customer acquisition, a stable product, and **under 10 hours a week** of management. That last bar matters: a company can't spin out if it still needs babysitting. The $5k isn't the goal — it's the point where a venture is real enough to stand on its own.

Click **Spinout Venture** and its BSSS ownership freezes into a formal cap table, it becomes an LLC, and it starts tracking real monthly economics — revenue, operating cost, profit distributed to owners by stake. An illustrative valuation (roughly 5× ARR) puts a paper value on everyone's holdings.

The cap table at the bottom pulls it together: for each holder, the paper value of their stakes, the cash they've drawn, the distributions they've collected from spun-out LLCs, and the total they've made — grouped into operations, capital, and investors, so you can see the three sides of the deal at once.

## What I left out on purpose

It's a teaching model, so it cuts corners honestly. Venture success is a hidden quality roll, not a real market. Valuations are a flat ARR multiple, not a real comp. The give-up percentages and funding amounts are knobs you set, not deals you negotiate. The aim was to make the flow understandable before making it accurate — and the labels say *simulated* everywhere for a reason.

Under the hood it's deliberately low-tech: one page of vanilla JavaScript, no build step, no framework, no backend. State lives in your browser, the ownership donuts are hand-drawn SVG, and the funnel and fund tank are plain CSS. Hover the **ⓘ** icons anywhere you're not sure what something means.

## Run it for sixty seconds

1. Set the raise target (or leave it at $300k) and **Fill Fund**.
2. **Advance One Month** a dozen times — watch the funnel fill, the fund drain, the donuts color in.
3. Open **Edit Participants**, give a contributor a deal — say $8k/month for 40% of their shares — and advance again to watch the investors' stake grow.
4. When a card turns green, **Spin it out** and see its ownership freeze into the cap table.

Do that and you'll feel the thing the model is really trying to teach: a venture studio is a portfolio machine, most of its ideas are meant to die, and the scarce resource the money actually buys is focus.

**[Run the simulator →](/venturestudio/)**
