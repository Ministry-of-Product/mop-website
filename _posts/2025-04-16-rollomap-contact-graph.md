---
layout: default
title: "RolloMap: A Contact Graph You Actually Own"
date: 2025-04-16
categories: ventures
permalink: /ventures/rollomap/
excerpt: Your address book lives on someone else's servers, silently rewriting your notes and disappearing if the company does. RolloMap is a local-first contact graph — every device keeps a full copy, every imported fact carries its provenance, and the sync runs on an open protocol you can self-host.
---

<div class="case-study-bar" style="background: var(--plate-rollomap);"></div>

# RolloMap: A Contact Graph You Actually Own

**[rollomap.com](https://rollomap.com)**

## The Challenge

The people you know are one of your most valuable assets, and almost nobody controls the record of them. Your contacts live inside a phone account, a CRM, or a social platform — systems that sync on their own terms, overwrite your careful notes with whatever a data provider last scraped, and hold your relationships hostage to a subscription. If the service shuts down or locks you out, the graph of who-you-know goes with it.

The deeper problem is trust. When a field changes, you can't tell whether *you* edited it or some import quietly did. There's no provenance, no offline guarantee, and no way to walk away with your own data intact.

## The Approach

We built RolloMap as a local-first contact graph, designed around a single principle: the data is yours, and the software should prove it.

**Every device keeps a complete copy.** The graph lives on your machine, not in a datacenter you rent access to. Offline always works because there is nothing to be offline *from* — the network is a convenience, not a dependency.

**Every imported fact carries its provenance.** When information comes in from an external source, RolloMap records where it came from. Nothing silently overwrites an edit you made by hand; you can always see who said what, and decide what to trust.

**Sync runs on an open, published protocol.** Because the protocol is documented rather than proprietary, clients and servers are interchangeable — anyone can build a compatible client, and no single vendor owns the pipe. The open-source client is free, and the whole stack can be self-hosted.

For people who'd rather not run infrastructure, **RolloMap Cloud** offers optional hosted sync, backup, and multi-device sharing for a flat monthly fee — a convenience layered on top, never a lock-in. If RolloMap Cloud disappeared tomorrow, you'd still own everything.

## The Outcome

RolloMap ships as an open-source, local-first application with an optional paid sync tier. It demonstrates that "you own your data" can be an architectural fact rather than a marketing line: ownership enforced by local copies, trust enforced by provenance, and portability enforced by an open protocol.

## What this demonstrates

Principled product architecture — starting from a value (data ownership) and letting it dictate the technical shape, rather than bolting privacy onto a cloud-first design after the fact. This venture shows how Ministry of Product approaches infrastructure products: pick the constraint that matters, build the system that makes it true by default, and give users a graceful on-ramp to convenience without ever taking the ownership away.
