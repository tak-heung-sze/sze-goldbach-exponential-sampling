# A Low-Variance Exponential Sampling Platform
## for Empirical Testing of the Hardy–Littlewood Goldbach Heuristic

**Tak Heung Sze**  
Independent Researcher

---

## Overview

This research introduces a deterministic exponential subsequence as a low-variance numerical
platform for empirical testing of asymptotic heuristics in additive prime number theory,
with specific focus on the Hardy–Littlewood Goldbach heuristic.

The study is methodological in nature and does not claim a proof of the Goldbach conjecture
nor any modification of the Hardy–Littlewood constants.

---

## Definition of the Sampling Sequence

We define the exponential subsequence

a(n) = 9 · 2^n,

referred to as the **Sze exponential sequence**.

For each N = a(n), we compute the number of Goldbach partitions g(N), defined as the number
of unique prime pairs (p, q) with p ≤ q such that p + q = N.

The empirical results are compared with the Hardy–Littlewood prediction E_HL(N),
including the singular series correction for divisibility by 3.

---

## Evaluation Metric

The primary quantity of interest is the ratio

R(N) = g(N) / E_HL(N).

Under the Hardy–Littlewood heuristic, this ratio is expected to converge slowly to 1
with deviations governed by an O(1 / ln N) error term.

---

## Key Empirical Observation

Sampling along the exponential subsequence a(n) = 9 · 2^n yields a notably stable ratio
series R(N) with reduced variance relative to sampling general even integers.

A matched control group restricted to the same modular class confirms that the observed
stability arises from variance reduction rather than additional arithmetic bias.

---

## Methodological Rationale

Empirical investigations of Goldbach-type heuristics typically suffer from large numerical
fluctuations at moderate scales.

This framework adopts a variance-reduction strategy based on:

- Exponential scaling, enabling large numerical ranges with modest index size.
- Fixed divisibility by 2 and 3, yielding a constant singular series contribution.
- Fully deterministic construction, ensuring complete reproducibility.

The objective is clarity of asymptotic observation rather than numerical enhancement.

---

## Scope and Limitations

- The analysis is restricted to a specific exponential subsequence.
- Results are finite-range and computationally bounded.
- No conjectural strengthening or probabilistic claims are made.

This work provides a clean empirical observation platform rather than a theoretical refinement.

---

## Repository Structure

```text
.
├── README.md
├── paper/
│   └── sze_goldbach_exponential_sampling_v1.pdf
├── data/        (optional; numerical tables)
├── src/         (optional; computation code)
└── results/     (optional; figures or derived outputs)
