---
title: "IoT Two-Factor Neurometric Authentication Using Wearable EEG"
excerpt: "My first lead-authorship paper. One thought does two jobs at once: it proves who you are, and it tells the device what to do."
date: 2019-05-23
categories:
  - Science
tags:
  - brain-computer interfaces
  - EEG
  - authentication
  - IoT
  - motor imagery
  - SafeThings 2019
---

## Background and inspiration

I loved the idea of interfacing directly with a computer — human expansion, the entity of our will wrapping around us like an exosuit and reaching into the digital ocean. *Ghost in the Shell*. Mechas. Iron Man. The Jaegers in *Pacific Rim*.

An early dream was to build technology that enabled that. But every version of it was contingent on two marvels of engineering: fusion, and brain-computer interfaces.

So when I sought out and received the opportunity to lead my own publication, I knew it would be about BCIs. Security was already baked into the lab expectation.

## Process

I dug into the realm of BCI security, narrowed down to BCI authentication, and read. A lot. I had to understand the state of the art, then the science underneath it, and then the math underneath *that*, which turned out to be highly relevant.

IoT TFNA itself is simple to state:

- We can identify, classify, and discriminate a brain signal read through EEG as one **motor imagery** out of a set — a user imagining rotating their hand at the wrist versus rotating their foot at the joint.
- We can also authenticate a user by having them think a **thought password**, differentiating their unique "mind-print" (mind finger print) from others.
- Lets can we build a system on that conjuction!

IoT TFNA uses a **single thought command** to send a secure instruction to an IoT device *inside the same packet used for authentication*. A randomized unique token adds an extra layer of security between source and endpoint.

IoT TFNA started as an effort to extend the state of the art. Then it became the way I got to dig into my own dreams via the industry interest I was begining to garner.

## Result

The poster edition was accepted to the **2019 IEEE SafeThings Workshop**, where I presented to an audience of guests from industry and academia. It is my first lead author papers to go on to publication - all during my undergrad career.

[Read the paper (PDF)](https://sararampazzi.com/doc/Rodriguez_eeg_SafeThings2019.pdf){: .btn .btn--primary}

## Where my head's at now

In-ear EEG carries so much more information per signal than is utilized by the scientific community. Some fresh eyed startup should explore that... ;)