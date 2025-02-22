---
title: 'Splicing'
summary: 'Splicing is the ability to resize Lightning channels on-the-fly, giving users of the Lightning Network many additional benefits that were not intuitively obvious at first.'
nym: 'Dusty Daemon'
website: 'https://lightningsplice.com/'
coverImage: '/static/images/projects/splicing.jpg'
git: 'https://github.com/lightning/bolts/pull/863'
twitter: 'dusty_daemon'
personalTwitter: 'dusty_daemon'
type: 'Other Free and Open-Source Project'
zaprite: '2qB3Y3gfSvOnWOv23BZb'
---

## About this project

Splicing is a proposal for BOLT 2, BOLT 7, and BOLT 9 that is maintained by
[Dusty Daemon](https://lightningsplice.com/dusty_daemon.html).

- See the complete proposal here: [Splicing Specification](https://github.com/lightning/bolts/pull/863/files)
- Discussion here: [Splicing Spec Conversation](https://github.com/lightning/bolts/pull/863)

At its core Splicing is a simple concept, the ability to resize Lightning
channels. But what's become apparent over time is the ability to resize
Lightning channels gives us many additional benefits that were not intuitively
obvious at first, and will fundamentally improve the utility of Lightning.

There are really two sides to what Splicing brings:

- User-facing improvements
- Backend liquidity improvements

Splicing is the process of moving a lightning channel's funding utxo into a new
"spliced" utxo. The exact steps involved are quite simple: sign the 2of2
multisignature transaction to a new location. Doing it in a trustless manner
however, is not simple at all.

- Splicing explained: [lightningsplice.com](https://lightningsplice.com/splicing_explained.html)
- Splicing video explanations: [lightningsplice.com/videos](https://lightningsplice.com/splicing_videos.html)

## About Dusty

I have been working on Bitcoin code for five years and 1.5 years ago I decided
to dedicate myself to programming for the Lightning network. I began by learning
about Lightning in depth and making contributions to the CoreLightning project.
I felt particularly accomplished rooting out some complex flakiness bugs and
porting the project to MacOS.

I had heard of splicing in 2018 and saw it making the news rounds last year. On
Clubhouse and Twitter Spaces bitcoiners were talking excitedly about using
submarine swaps and I suggested people use splicing instead! The confused
silence was palpable, no one had heard about it all. Diving in I realized only
the splicing spec had been released — no one had actually written the code! So I
decided I would take on the work of coding up the first implementation. By March
of this year I had made the world’s first splice and published it on chain! You
can see it here:
[twitter](https://twitter.com/dusty_daemon/status/1522413475909316610),
[mempool](https://mempool.space/tx/c143bbd3f983e7d07bbccf571352c2432c8e97a543d26a6962582021ec788804).

Since then I have been working on finishing up the proper & complete splice
implementation. The code is now in a beta state which you can see here:
[PR #5675](https://github.com/ElementsProject/lightning/pull/5675)

I’m looking for funding to finish the code to a polished state, build a thorough
testing framework, evangelize to companies that would benefit from splicing, and
bring the implementation to the other Lightning node code bases.

- Dusty's worklog: [ddustin/worklog](https://github.com/ddustin/worklog)
