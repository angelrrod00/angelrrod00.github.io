---
title: "Trick or Heat? Attacking Temperature Control With a Radio"
excerpt: "My first paper. No code, just a software-defined radio and physics — and what happens when the sensor feeding a control loop can be told what to say."
date: 2019-11-11
categories:
  - Science
tags:
  - sensor security
  - cyber-physical systems
  - electromagnetic interference
  - SPQR Lab
  - CCS 2019
---

## Background and inspiration

In the summer of 2018 I decided to give myself a shot at my dream of being a scientist and a researcher. I had okay grades and, from my perspective, *no* experience. I applied to the position anyway.

When I got the interview with Dr. Sara Rampazzi I was surprised, nervous, and afterward certain I had not gotten it.

I count taking that chance as another one of my "greatest accomplishments" — because I never expected that a single choice would produce my greatest friends, my greatest times, and many more of my greatest accomplishments.

I was hired to conduct laboratory experiments in the SPQR Lab at the University of Michigan College of Engineering.

## Process

The idea was simple. Wires, traces, and conductors carry a measurable induced current in a changing magnetic field. Your microwave messes with the TV. Your cell phone messes with your speakers. And if you have ever worked with raw signals, you know that noise filtering is a front-loaded expectation before you can extract anything useful at all.

So: what if we intentionally fire radio waves *into* sensitive sensors?

And further — if that sensors' system is guiding logic, can we gain the ability to exploit the logic itself?

No code. Just a walkie-talkie and physics.

My role on the project:

- Running the "walkie" — a USRP software-defined radio
- Building our sensor system test bed
- Writing sections of the paper, and reviewing others
- Coordinating between our lab partners across two universities
- Presenting the idea for the mitigation system, and collaborating on its refinement

## Result

The work became a paper at ACM CCS 2019 in London. We showed that an adversary can remotely manipulate the temperature readings of a critical system — an infant incubator among them — by inducing an unintended rectification effect in the operational and instrumentation amplifiers that condition the sensor signal. The control loop heats or cools on command, without the attacker touching the device. The same hardware-level weakness reaches other classes of sensors that share a similar signal conditioning path. Because conventional defenses were not enough, we proposed a low-cost anomaly detector to protect the integrity of the sensor signal.

> Yazhou Tu, Sara Rampazzi, Bin Hao, **Angel Rodriguez**, Kevin Fu, and Xiali Hei. "Trick or Heat? Manipulating Critical Temperature-Based Control Systems Using Rectification Attacks." *Proceedings of the 2019 ACM SIGSAC Conference on Computer and Communications Security (CCS '19)*, London, United Kingdom, pp. 2301–2315.

[ACM Digital Library](https://dl.acm.org/doi/10.1145/3319535.3354195){: .btn .btn--primary}
[Preprint (arXiv)](https://arxiv.org/abs/1904.07110){: .btn .btn--inverse}

## Where my head's at now

This was my first paper, and I loved it. It is also the project that permanently changed how I look at a embedded systems: the specified behavior on the datasheet of components is a narrowed description of the system, guessed (see: industry) and under ideal conditions.
