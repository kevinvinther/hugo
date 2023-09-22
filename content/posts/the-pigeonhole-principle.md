---
title: "The Pigeonhole Principle"
date: 2023-09-22T09:50:22+02:00
draft: false
---

# Introduction

The pigeonhole principle is a mathematical principle and counting argument,[^1] which is often accompanied with the hypothetical scenarios of pigeons and pigeonholes (from which the name comes). 

Imagine you have $n+1$ pigeons, and $n$ pigeonholes. The pigeonhole principle states that, since there is one more pigeon than there is pigeonholes, **at least** one of the pigeonholes must hold two pigeons. 

For example, if you have 11 pigeons and 10 pigeonholes, or equivalently, 11 pencils and 10 pencil cases, then at least one of the pigeonholes or pencil cases must hold 2 pigeons or pencils, respectively.

Now, what would happen if we had 21 pencils but only 10 pencil cases?

# Generalization

We can generalize the principle. Imagine you have $n$ pencils, and $k$ pencil cases. Then, according to the generalized pigeonhole principle, there is at least one pencil case containing $\lceil n / k \rceil$[^2] pencils.

Referring back to the question from earlier, consider having 21 pencils, but only 10 pencil cases. The generalization of the pigeonhole principle then shows us that there must be $\lceil 21 / 10 \rceil = 3$  pencils in one of the pencil cases.

# Use in Proofs

Now, while this is very simple and may seem very intuitive, it can be powerfully used in proofs. For example, take the proof of the following theorem: 

Every sequence of $n^2 + 1$ distinct real numbers contains a subsequence of length $n+1$ that is either strictly increasing or strictly decreasing. 

Consider the proof for this theorem:[^3]
Let $a_1, a_2, ..., a_{n^2+1}$ be a sequence of distinct real numbers. Associate an **ordered pair**  $(i_k, d_k)$ with each term of the sequence, $a_k$. Here $i_k$ is the length of the longest *increasing* subsequence starting at $a_k$, and $d_k$ is the longest *decreasing* subsequence starting at $a_k$.
Now, suppose that there are no increasing nor decreasing subsequences of length $n+1$. Then $i_k$ and $d_k$ are both positive integers less than or equal to $n$, for $k = 1, 2, ..., n^2 +1$. Hence, by the product rule,[^4] there are $n^2$ possible ordered pairs for $(i_k, d_k)$. 
Now comes the part where we use the pigeonhole principle. By the pigeonhole principle, two of these $n^2 + 1$ ordered pairs are equal as there are only $n^2$ possible ordered pairs, but we have $n^2 + 1$ elements. 
In other words, there exists two different terms $a_s$ and $a_t$, where $s < t$, such that $i_s = i_t$ and $d_s = d_t$. 
We will show that this is impossible. Because the terms of the sequence are distinct, either $a_s < a_t$ or $a_t > a_s$. Then if $a_s < a_t$, because $i_s = i_t$, an increasing subsequence of length $i_t + 1$ can be built starting at $a_s$, by taking $a_s$ followed by an increasing subsequence of length $i_t$ beginning at $a_t$. This is a contradiction, as we supposed that there were no subsequences of length $n+1$, yet we found one. If $a_s > a_t$ the same reasoning shows that $d_s$ must be greater than $d_t$, which is a contradiction. This concludes the proof.

# Proofs of the Principles

**The Pigeonhole Principle**:
We use a proof by contraposition. Assume that there must be **at most** 1 pigeon per pigeonhole. Then the maximum number of pigeons is $n$. This contradicts our initial assumptions that there are $n+1$ pigeons. This concludes the proof.

**The Generalized Principle**:
Assume we only have at most $\lceil n/k \rceil - 1$   pigeons per pigeonhole. Then the number of pigeons must be $k(\lceil n/k \rceil - 1)$. However, 
$$k\left( \left \lceil \frac{n}{k} \right \rceil - 1\right) < k\left (\left (\frac{n}{k} +1 \right ) - 1\right)$$
where the inequality $\lceil n/k \rceil < (n/k)+1$[^5] has been used. 
This shows that, if we indeed assume that each pigeonhole has at most $\lceil n/k \rceil - 1$ pigeons, then the total number of pigeons must be strictly less than $k(n/k)$ which is the total number of pigeons. This is a contradiction, as it claims that the number of pigeons is less than $n$, but there are $n$ pigeons. This concludes the proof.

# Conclusion

In conclusion, the pigeonhole principle, while seemingly simple and intuitive, serves as a potent tool in mathematical proofs.

[^1]: A counting argument proves statements by counting objects in two different ways, showing that the two counts must be equal
[^2]: The ceiling function ($\lceil x \rceil$) maps the value $x$ to its nearest integer greater than or equal to $x$.
[^3]: This proof is from Discrete Mathematics and its Applications, Eighth Edition by Kenneth Rosen
[^4]: If there are $n_1$ ways to do task one of two, and for each of these ways, there are $n_2$ ways to do the second task, then there are $n_1n_2$ ways to do the procedure.
[^5]: The inequality $\lceil n/k \rceil < (n/k)+1$ holds because the ceiling functions always rounds a non-integer value up to the nearest integer.
