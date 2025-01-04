---
title: "An Analysis of Speculative Type Confusion Vulnerabilities in the Wild"
date: 2021-11-24
time: 3PM
presenter: "adam-morrison"
youtube: "gLGUnIfXNRY"
zoom-link: "https://newcastleuniversity.zoom.us/j/82801486439?pwd%3Dd2NhMlJwMmxMaFlsWkhMak5qVXBlQT09"
zoom-id: "828 0148 6439"
zoom-password: "165033"
---

Spectre v1 attacks, which exploit conditional branch misprediction, are often identified with attacks that bypass array bounds checking to leak data from a victim's memory. Generally, however, Spectre v1 attacks can exploit any conditional branch misprediction that makes the victim execute code incorrectly. In this paper, we investigate speculative type confusion, a Spectre v1 attack vector in which branch mispredictions make the victim execute with variables holding values of the wrong type and thereby leak memory content.

We observe that speculative type confusion can be inadvertently introduced by a compiler, making it extremely hard for programmers to reason about security and manually apply Spectre mitigations. We thus set out to determine the extent to which speculative type confusion affects the Linux kernel. Our analysis finds exploitable and potentially-exploitable arbitrary memory disclosure vulnerabilities. We also find many latent vulnerabilities, which could become exploitable due to innocuous system changes, such as coding style changes.

Our results suggest that Spectre mitigations which rely on statically/manually identifying “bad” code patterns need to be rethought, and more comprehensive mitigations are needed.