# A Low-Variance Exponential Sampling Platform  
## for Empirical Testing of the Hardy–Littlewood Goldbach Heuristic

**Tak Heung Sze**  
Independent Researcher  

---

### Abstract

We introduce a structured exponential subsequence designed as a low-variance numerical platform for empirical testing of asymptotic heuristics in additive prime number theory. Focusing on Goldbach partition counts, we study the sequence

\[
a(n) = 9 \cdot 2^n ,
\]

referred to as the *Sze exponential sequence*.  
For each \( N = a(n) \), we compute the number of Goldbach partitions \( g(N) \) and compare it with the Hardy–Littlewood prediction \( E_{\mathrm{HL}}(N) \), including the singular series correction.

We show that this exponential subsequence yields a notably stable ratio

\[
R(N) = \frac{g(N)}{E_{\mathrm{HL}}(N)},
\]

with reduced variance relative to general even integers.  
A matched modular control confirms that the observed stability arises from variance reduction rather than additional arithmetic bias.

---

### 1. Scope of the Repository

This repository serves as a **research artifact** accompanying the paper:

> *A Low-Variance Exponential Sampling Platform for Empirical Testing of the Hardy–Littlewood Goldbach Heuristic*

The contribution is **methodological**.  
No claim is made regarding a proof of the Goldbach conjecture or modification of the Hardy–Littlewood heuristic.

---

### 2. Repository Structure

```text
.
├── README.md
├── paper/
│   └── sze_goldbach_exponential_sampling_v1.pdf
├── data/        (optional; numerical
