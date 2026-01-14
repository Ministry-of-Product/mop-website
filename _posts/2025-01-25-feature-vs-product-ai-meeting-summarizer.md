---
layout: abl_post
title: "Feature vs Product: AI Meeting Summarizer"
date: 2025-01-25
categories: always-be-launching
what_they_built: "An AI tool that joins Zoom meetings, transcribes them, and generates summaries with action items. The prototype integrates with Zoom's API, uses Whisper for transcription, and GPT-4 to create structured summaries. It works reliably and produces good output."
original_assumption: "The builder assumed this was a standalone product that people would pay for monthly. They built user accounts, meeting scheduling, email notifications, and a web dashboard to view summaries. The assumption was that busy professionals would pay $19/month to never take meeting notes again."
where_they_got_stuck: "The tool worked. Early users liked the summaries. But when asked to pay, most said they'd 'think about it' or that their company 'already has something for that.' The builder kept adding features: integration with more video platforms, better formatting, team sharing. But conversion stayed low. They weren't sure if this was a product, a feature of something larger, or just not valuable enough."
decision_that_mattered: "The decision that mattered was recognizing that meeting summarization is usually a feature, not a product. Most companies already have meeting tools (Zoom, Teams, etc.) and those tools are adding AI summarization. The builder needed to either: (1) target a specific niche where meeting summaries are the core need (like therapy sessions or legal consultations), or (2) accept that this is a feature and find a larger product to attach it to. Trying to sell it as a standalone product was fighting against how people actually use meeting tools."
what_should_happen_next: "Stop building more integrations. Pick one: either narrow to a specific use case where summaries are the core value (not just nice-to-have), or pivot to building something larger where meeting summaries are one feature. If you go narrow, focus on a vertical where people actually need detailed meeting records: therapists, lawyers, consultants doing client calls. If you go broad, think about what else people need around meetings: scheduling, follow-ups, relationship management. But don't keep building a standalone summarization tool—that's a feature, not a product."
patterns:
  - Feature vs product
  - No clear user
  - Overbuilt too early
excerpt: "An AI meeting summarizer that works well but struggles because meeting summaries are usually a feature of larger tools, not a standalone product people will pay for."
---

## The Full Story

This builder created a reliable AI meeting summarizer. It worked well. The summaries were accurate. Early users gave positive feedback.

But when it came time to convert to paid subscriptions, most people said their company already had something for that, or they'd think about it later. The builder kept improving the tool, adding more features, thinking the problem was functionality.

The real problem was positioning. Meeting summarization is becoming a standard feature in video conferencing tools. Zoom, Teams, and others are building this in. Trying to sell it as a standalone product means competing against features that are free with tools people already use.

The builder needed to either find a niche where summaries are the core value (not just convenient), or accept that this is a feature and build something larger around it.

## Key Insight

If your product feels like it should be a feature of something people already use, it probably is. Either find a niche where it's the core value, or build the larger thing it belongs to.

