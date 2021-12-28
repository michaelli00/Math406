# Chapter 2

\# 8, 9, 10, 12, 13, 14, 20*, 24*, 28*, 30, 32*, 35, 41, 42, 43, 44, 45, 47, 67, 76, *86

**8\.** 

Divisors of $12 = \{1, 2, 3, 4, 6\}$

Divisors of $13 = \{1, 13\}$

Divisors of $15 = \{1, 3, 5, 15\}$

Divisors of $16 = \{1, 2, 4, 8, 16\}$

**9\.**

$6 \nmid a$ and $6 \nmid b \implies 6 \nmid ab$ is false since $6 \nmid 3$ and $6 \nmid 2$ but $6 \nmid 2*3$

$6 \nmid a$ and $6 \nmid b \implies 36 \nmid ab$ is false since $6 \nmid 4$ and $6 \nmid 9$ but $6 \mid 4 * 9$

$6 \nmid a$ and $6 \nmid b \implies 6 \nmid (a + b)$ is false since $6 \nmid 4$ and $6 \nmid 2$ but $d \mid (2 + 4)$

**10\.**

$6 \mid a$ and $6 \mid b \implies 6 \mid ab$ is true since $a = 6k_1$ and $b = 6k_2 \implies ab = 36k_1k_2 \implies 6 \mid ab$

$6 \mid a$ and $6 \mid b \implies 36 \mid ab$ is true since $a = 6k_1$ and $b = 6k_2 \implies ab = 36k_1k_2 \implies 36 \mid ab$

**12\.**

Sum of 2 even numbers is even: Let $n = 2k_1$ and $m = 2k_2$. Then $n + m = 2(k_1+k_2)$ which is even

Sum of 2 odd numbers is even: Let $n = 2k_1 + 1$ and $m = 2k_2 + 1$. Then $n + m = 2(k_1 +k_2 + 1)$ which is even

Product of 2 even numbers is even and divisible by $4$: Let $n = 2k_1$ and $m = 2k_2$. Then $nm = 4k_1 k_2$ which is even and divisible by $4$

Product of 2 odd numbers is odd: Let $n = 2k_1 + 1$ and $m = 2k_2 + 1$. Then $nm = 2(2k_1k_2 + k_1 + k_2) + 1$ which is odd

**13\.** Find all $n \in Z$ such that $n^2 - n$ is prime

Only $n \in \{-1, 2\}$ work since these generate $n^2 - n = 2$. All other $n \in Z$ do not work since either we get odd - odd is even and divisible by $2$ or even - even and divisible by $2$

**14\.** Show that if $n \in Z$ then $2 \mid n^2 - n$

Proof by cases:

- Let $n$ be odd and $n = 2k + 1$. Then $n^2 - n = 2(2k^2 + 3k + 1)$ which is divisible by $2$
- Let $n$ be even and $n = 2k$. Then $n^2 - n = 2(2k^2 -k)$ which is divisible by $2$

**20\.** Let $a, b \in Z$ be nonzero such that $a \mid b$ and $b \mid a$. Show that $a = \pm b$

We know that $a = bk_1$ and $b = ak_2 \implies a = a k_1k_2 \implies k_1 k_2 = 1$.

Since $k_1, k_2 \in Z \implies k_1 = k_2 = \pm 1$

Thus $a = b * \pm 1= \pm b$

**24\.** Show that for $n \geq 2$, each of $n! + 2, n! + 3, n! + 4, \ldots, n! + n$ is composite

Clearly $n \mid n! + 2$. Thus each one is composite

**28\.** Prove or disprove that the difference of cubes of successive positive integers is always prime

False: $6^3 - 5^3 = 91 = 7 * 13$

**32\.**: Prove that there are infintely many even integers that are sums of two primes

Since there are an infinite number of (odd) primes, there are an infinite number of addition pairs of these primes, and thus an infinite number of even integers the sume of two primes

**35\.**

$29 = 14*2 + 1$

$53 = 8 * 6 + 5$

$205 = 15 * 13 + 10$

$45 = 9 * 5 + 0$

**41\.** Today is Monday. What day of the week will it be in 100 days?

$100 \pmod{7} = 2 \implies$ it will be Wednesday

**42\.** It is July. What month will it be 100 months from now?

$100 \pmod{12} = 4 \implies$ it will be November

**43\.**

$1! + 2! + 3! + \cdots + 100! / 7 \equiv 873 \pmod{7} = 5$

$1! + 2! + 3! + \cdots + 100! / 8 \equiv 6 \pmod{8}$

**45\.** Find all $n \in Z$ such that $n^2 + 1$ is divisible by $n + 1$

$n \in \{0, 1\}$ all other values don't work since if $n$ is odd, we have even / odd. If $n$ is even, we have odd / even


**67\.** Use Extended Euclidean Algorithm for $\gcd(182, 630)$ and write the $\gcd$ as a linear combination of $182, 630$

$$630 = 3*182 + 84$$
$$182 = 2*84 + 14$$
$$84 = 6 *14 + 0$$

|       | $x$ | $y$   |    |
| ------| ----| ----  | -- |
| $630$ | $1$ | $0$   |    |
| $182$ | $0$ | $1$   |    |
| $84$  | $1$ | $-3$  | $R_1 - 3R_2$   |
| $14$  | $-2$| $7$   | $R_2 - 2*R_3$   |

Thus $\gcd(182, 630) = 14 = -2 * 630 + 7 * 182$

**86\.** Show that if $n \in Z^+$ such that $(3^n - 1)/2$ is prime, then $n$ is prime

By contradiction, suppose $n$ is composite so $n = ab$. Then let $x = 3^a$ and $k = b$

Then $3{ab} - 1) = (3^a - 1)(3^{a(b-1)} + \cdots + 3^a + 1)$

$1 < a < n \implies 1 < 3^a - 1< 3^n - 1$ so $3^{a} - 1$ is a nontrivial factor and $3^n - 1$ is composite
