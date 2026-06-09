---
layout: post
title: Invited Talk at AViD Workshop 2026
date: 2026-05-17 10:00:00-0400
description: Efficient Zero-Knowledge Proofs for AI Inference
---

I gave an invited talk on **Efficient Zero-Knowledge Proofs for AI Inference** at the [AViD (Assurance & Verification of AI Development) Workshop](https://www.far.ai/news/avid-workshop-2026), organized by FAR.AI, Center for AI Safety, and Longview Philanthropy on May 17, 2026.

<div style="text-align: center;">
<img src="/assets/img/avid_workshop.jpg" alt="Speaking at AViD Workshop 2026" style="width: 100%;">
</div>

<br>

As AI moves into high-stakes domains like medical diagnosis, we need verifiable evidence that AI services actually ran the claimed model. Zero-knowledge machine learning (zkML) addresses this by using cryptographic proofs to certify correct AI inference while keeping model weights confidential. However, the prover overhead has been a major bottleneck (>1000x compared to plaintext inference).

In this talk, I presented our recent work that achieves a **10x improvement** over the state of the art, reducing GPT-2 per-token prover time to **1.5 seconds** (down from 3600s just three years ago). Our key techniques include:
- A compiler that unifies diverse linear operations (MatMul, attention, etc.) into a **single ZKP constraint**
- **Sublinear-time proving** (in the lookup table size) for exponentiation-related nonlinearities (e.g., softmax) by exploiting the special structure of lookup tables
- Systems optimizations including batching and parallel proof computation

The full playlist of talks is available on [YouTube](https://www.youtube.com/playlist?list=PLpvkFqYJXcrdMuk0zgy0x6RWn8Ssq3R5v).
