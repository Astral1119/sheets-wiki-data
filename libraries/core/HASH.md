---
tags:
  - anduin
---

`HASH` is a [hashing function](https://en.wikipedia.org/wiki/Hash_function) designed for compatibility with Anduin containers. Inputs are hashed to an eight-digit [base-36](https://en.wikipedia.org/wiki/Base36) string.

### Collision

Hashes, by nature of mapping an infinite input domain to a restricted output, have a probability of [collision](https://en.wikipedia.org/wiki/Hash_collision). In order to calculate the probability of collision, we can use an approximation of the [birthday problem](https://en.wikipedia.org/wiki/Birthday_problem), derived from its Taylor series expansion.

$$
p(k)\approx 1-e^{-{\frac {k^{2}}{2n}}}
$$
Where $n$ is the cardinality of the hash space, or $36^8 \approx 2.8 \text{ trillion}$.

| $k$ (Number of items) | Probability of collision |
| --------------------- | ------------------------ |
| 1000                  | 0.0000001772351919       |
| 10000                 | 0.0000177233637          |
| 100000                | 0.001770782387           |
| 1000000               | 0.1624172444             |
| 2000000               | 0.507834792              |
| 5000000               | 0.9880959927             |

This approximation only holds as long as the hash function follows a [continuous uniform distribution](https://en.wikipedia.org/wiki/Continuous_uniform_distribution). Below is an empirical result from hashing two datasets, showing that it does.

![[Distribution of hash characters on two datasets.svg]]