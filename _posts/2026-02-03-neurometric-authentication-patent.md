---
title: "US Patent 12,541,676 — Neurometric Authentication System"
excerpt: "My first patent, and the continuation of IoT TFNA: macro commands, an air-gapped verification path, and intention as the identifier."
date: 2026-02-03
categories:
  - Engineering
tags:
  - patent
  - brain-computer interfaces
  - EEG
  - authentication
  - ASIC
---

## Background and inspiration

This is my first patent, and it carries the same name as the work it grew out of. Out of the paranoia I was gifted from SPQR I set out to design an end to end secure BCI. It begged the question: what is secure, what is an interface, and what is the root chain we can trust as "intention".

## Process

The build-out beyond the publication included two major additions:

**Macro commands.** M measured neurological impulse resolves to N^M macro commands where N is the resolution of (or number of symbols in) the BCI's language. 

**Intention as the identifier.** The thing that distinguishes one user of the device from another is not a stored credential but the shape of the intention itself - a derived "mind-print", constantly verified.

The described system of systems allows for multimodal acquisition, the security guarantees of an isolated air-gapped verification path, and implied ingenious UIs built on top.

The claimed pipeline runs: sensors generate voltage signals from a measured neurological impulse → ASICs digitize them → an activation command wakes the device from an energy-efficient mode into an active mode → the signal is encoded from the time domain into the frequency domain (via FFT or Riemannian geometry) → a support-vector machine or convolutional neural network classifies it → the resulting macro command is encoded into a token alongside verification data derived from a random seed → the token is broadcast, and the destination device verifies it with a server before acting.

## Result

- **Patent number:** US 12,541,676 B2
- **Title:** Neurometric authentication system
- **Inventor:** Angel Raphael Rodriguez (sole)
- **Priority date:** January 20, 2020
- **Filed:** January 20, 2021
- **Published as application:** US 2021/0224637 A1, July 22, 2021
- **Granted:** February 3, 2026

[Read on Google Patents](https://patents.google.com/patent/US12541676B2){: .btn .btn--primary}

## Where my head's at now

TODO