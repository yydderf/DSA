---
description: https://open.kattis.com/contests/vaucue/problems/kinversions
---

# K-Inversions

### Initial Thoughts

* 1 000 000 -> brute force (n^2) would result in TLE
* merge sort would scramble the order

***

### Solve

* index the position of A's and B's
* convert the index to polynomials (A as positive, B as negative)
* multiply the polynomials

Example: BABA

* BABA, index B = {0, 2}, index A = {1, 3}
* A= {1, 3} = g(x) = x + x^3
* B = {0, 2} = f(x) = 1 + x^-2
* h(x) = f(x)g(x) = x + x^-1 + x^3 + x = x^-1 + 2x + x^3

