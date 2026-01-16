# A Low-Variance Exponential Sampling Platform for Empirical Testing of the Hardy-Littlewood Goldbach Heuristic

## 📝 Abstract
This project introduces a structured exponential subsequence, the **Sze Exponential Sequence**, designed as a low-variance numerical platform for testing asymptotic heuristics in additive prime number theory. By focusing on Goldbach partition counts, this framework provides a clean and reproducible environment for observing convergence behavior.

## 🧮 Mathematical Definition

### 1. The Sze Exponential Sequence
The sequence is defined as:

$$a(n) = 9 \cdot 2^{n}$$

where $n \in \mathbb{N}$.

### 2. Evaluation Metric
The primary evaluation metric is the ratio between the exact Goldbach partitions $g(N)$ and the Hardy-Littlewood prediction $E_{HL}(N)$:

$$R(N) = \frac{g(N)}{E_{HL}(N)}$$

The prediction $E_{HL}(N)$ is calculated as:

$$E_{HL}(N) = 2C_{2} \frac{N}{(\ln N)^{2}} \mathfrak{S}(N)$$

Where:
* $C_{2}$ is the twin prime constant.
* $\mathfrak{S}(N)$ is the singular series correction.

## 🌟 Key Properties
The Sze exponential sequence exhibits three properties relevant to empirical testing:
* **Exponential Scaling**: Enables testing across large numerical ranges with modest $n$.
* **Fixed Modular Structure**: Constant divisibility by 2 and 3 yields a stable singular series contribution.
* **Deterministic Construction**: Ensures full reproducibility of results.
* **Variance Reduction**: Provides a stable ratio series with reduced variance relative to general even integers.

## 📊 Experimental Results
Across the tested range ($N \approx 10^{4}$ to $10^{9}$), the following results were observed:
* **Stability**: The ratio $R(N)$ remained within the range $[0.56, 0.68]$.
* **Mean Ratio**: The average ratio was observed at $\overline{R} = 0.604 \pm 0.04$.
* **Consistency**: Results are consistent with the expected $O(1/\ln N)$ asymptotic convergence predicted by the Hardy-Littlewood heuristic.

## 🚀 Future Roadmap
* **Extended Range**: Future work aims to extend the range toward $n=50$ ($N \approx 10^{15}$).
* **Parallel Computation**: Implement optimized, WebAssembly-based parallel computation frameworks.

## 📚 Citation
If you use this work, please cite it as follows:
> **Sze, T. H.** (2026). *A Low-Variance Exponential Sampling Platform for Empirical Testing of the Hardy-Littlewood Goldbach Heuristic*. Independent Researcher.
