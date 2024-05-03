---
description: Cooley-Turkey FFT
---

# Fast Polynomial Multiplication

### Description

* coefficient f(x), g(x) -> point-value f(x), g(x) \[O(nlogn)]
* point-value multiplication -> h(x) \[O(n)]
* point-value h(x) -> coefficient h(x) \[O(nlogn)]

f(x): (0, 2), (1, 1), (2, 3), (3, 0)

g(x): (0, 4), (1, 3), (2, 1), (3, 0)

f(x)g(x): (0, 8), (1, 3), (2, 3), (3, 0)

### Reference

* [https://cp-algorithms.com/algebra/fft.html](https://cp-algorithms.com/algebra/fft.html)

### Problems

* [k-inversions.md](problems/k-inversions.md "mention")
