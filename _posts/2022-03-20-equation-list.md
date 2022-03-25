---
layout: post
title: "The Ultimate Equation List"
tags: [CP, Monstrous]
usemathjax: true
featured: true
---
Hi, I am super excited to be back with another ultimate list. This time it is a collection of all important equations in Competitive Programming.

### Motivation
Do you find it bad if you couldn’t solve a problem just because you didn’t know about a certain equation? 

Do you find it difficult to take a quick look at an equation that you know exists but forgot about it while solving a problem?

Do you think that all the equations that are important in CP are just cluttered and you are too lazy to collect them in one place?

Well, then you are in the right place! I am here to solve all of the aforementioned problems. I believe you should not waste your precious time searching the internet for important equations. You should solve more problems. I am here to undertake the nasty task of collecting things. 

### Payment
Everything comes with a cost. You need to do something for me. That is you need to upvote my Codeforces blog of this list! The link to the blog: TBA

### Acknowledgement
Thanks to the following guys as they converted all the equations to Latex: Mahbubul Alam Sabuj(CF: newb_ie), Irfan Ullah Munna (CF: Shanto65), S.M.A Nahian (CF: Nahian9696), Ashiqur Rahman Naeem (CF: nayeem2021), Md. Imran Hossain(CF: peripatetic), Jamilur Rahman(CF: Jamil314) and Mahmood (CF: mah_mood).

### About the List
I didn't add any explanations for any of the equations because its not feasible to explain too many equations. So make sure to understand them by yourself or use google or just comment under this blog. The community will help.

The list also contains some small tricks as a bonus. As the list is long, it must have some errors. Feel free to point those out.

Enjoy!

### The Equation List

### Combinatorics

#### General
1. $\displaystyle \displaystyle \sum \limits_{0\leq k \leq n} {n-k \choose k} = Fib_{n+1}$
2. $\displaystyle \displaystyle {n \choose k}={n \choose n-k}$
3. $\displaystyle \displaystyle {n \choose k}+{n \choose k+1}={n+1 \choose k+1}$
4. $\displaystyle \displaystyle k{n \choose k}=n{n-1 \choose k-1}$
5. $\displaystyle \displaystyle {n \choose k}=\frac{n}{k}{n-1 \choose k-1}$
6. $\displaystyle \sum \limits_{i=0}^n{n \choose i}=2^n$
7. $\displaystyle \sum \limits_{i\geq 0}{n \choose 2i}=2^{n-1}$
8. $\displaystyle \sum \limits_{i\geq 0}{n \choose 2i+1}=2^{n-1}$
9. $\displaystyle \sum \limits_{i= 0}^k \left( -1 \right) ^i{n \choose i}=\left( -1 \right) ^k{n-1 \choose k}$
10. $\displaystyle \sum \limits_{i= 0}^k{n+i \choose i}={n+k+1 \choose k}$
11. $\displaystyle \sum \limits_{i= 0}^k{n+i \choose n}={n+k+1 \choose k}$
12. $\displaystyle \sum \limits_{i= 0}^k{i \choose n}={k+1 \choose n+1}$
13. $\displaystyle \displaystyle1{n \choose 1}+2{n \choose 2}+3{n \choose 3}+...+n{n \choose n}=n2^{n-1}$
14. $\displaystyle \displaystyle1^2{n \choose 1}+2^2{n \choose 2}+3^2{n \choose 3}+...+n^2{n \choose n}=(n+n^2)2^{n-2}$
15. **Vandermonde's Identify:** $\displaystyle \sum \limits_{k=0}^r{m \choose k}{n \choose r-k}={m+n \choose r}$
16. **Hockey-Stick Identify:** $\displaystyle \ n,r \in N, n > r, \sum \limits_{i=r}^n{i \choose r}={n+1 \choose r+1}$
17. $\displaystyle \sum \limits_{i=0}^k{k \choose i}^2={2k \choose k}$
18. $\displaystyle \sum \limits_{k=0}^n{n \choose k}{n \choose n-k}={2n \choose n}$
19. $\displaystyle \sum \limits_{k=q}^n{n \choose k}{k \choose q}=2^{n-q}{n \choose q}$
20. $\displaystyle \sum \limits_{i=0}^n3^i{n \choose i}=4^n$
21. $\displaystyle \sum \limits_{i=0}^nk^i{n \choose i}=(k+1)^n$
22. $\displaystyle \sum \limits_{i=0}^n{2n \choose i}=2^{2n-1}+\frac{1}{2}{2n \choose n}$
23. $\displaystyle \sum \limits_{i=1}^n{n \choose i}{n-1 \choose i-1}={2n-1 \choose n-1}$
24. $\displaystyle \sum \limits_{i=0}^n{2n \choose i}^2=\frac{1}{2} \left( {4n \choose 2n}+{2n \choose n}^2 \right)$
25. **Highest Power of $\displaystyle 2$ that divides $^{2n}C_n$:**
    Let $\displaystyle x$ be the number of $\displaystyle 1$s in the binary representation. Then the number of odd terms will be $\displaystyle 2^x$.Let it form a sequence. The $n$-th value in the sequence (starting from $n$ = 0) gives the highest power of $\displaystyle 2$ that divides $^{2n}C_n$.
26. **Pascal Triangle**
    1. In a row $\displaystyle p$ where $\displaystyle p$ is a prime number, all the terms in that row except the $\displaystyle 1$s are multiples of $\displaystyle p$.
    2. Parity: To count odd terms in row $n$, convert $n$ to binary. Let $\displaystyle x$ be the number of $\displaystyle 1$s in the binary representation. Then the number of odd terms will be $\displaystyle 2^x$.
    3. Every entry in row $\displaystyle 2^n-1, n\geq 0,$ is odd.
27. An integer $n\geq 2$ is prime if and only if all the intermediate binomial coefficients $\displaystyle \displaystyle {n \choose 1},{n \choose 2},..., {n \choose n-1}$ are divisible by $n$. 
28. **Kummer's Theorem:** For given integers $n\geq m\geq 0$\displaystyle \ and a prime number $\displaystyle p$, the largest power of $\displaystyle p$ dividing $\displaystyle \displaystyle {n \choose m}$  is equal to the number of carries when $m$ is added to $n$-$m$ in base $\displaystyle p$. For implementation take inspiration from lucas theorem.
29. Number of different binary sequences of length $n$ such that no two $0$’s are adjacent=$\displaystyle Fib_{n+1}$
30. **Combination with repetition:** Let’s say we choose $\displaystyle \displaystyle k$ elements from an $n$-element set, the order doesn’t matter and each element can be chosen more than once. In that case, the number of different combinations is: $\displaystyle \displaystyle {n+k-1 \choose k}$
31. Number of ways to divide $n$ persons in $\displaystyle \frac{n}{k}$ equal groups i.e. each having size $\displaystyle \displaystyle k$ is 
    
    $$
    \displaystyle \frac{n!}{k!^{\frac{n}{k}} \left( \frac{n}{k} \right) !}= \prod \limits_{n \geq k}^{n-=k}{n-1 \choose k-1}
    $$
32. The number non-negative solution of the equation: $\displaystyle x_1+x_2+x_3+...+x_k=n \text{ is}{n+k-1 \choose n}$
33. Number of ways to choose $n$ ids from $\displaystyle 1$ to b such that every id has distance at least k  $\displaystyle \displaystyle =\left( \frac{b-(n-1)(k-1)}{n} \right)$  
34. $\displaystyle \displaystyle \sum \limits_{i=1,3,5,\dots}^{i\leq n} \binom{n}{i} a^{n-i}b^i = \frac{1}{2} ((a+b)^n-(a-b)^n)$
35. $\displaystyle \displaystyle \sum \limits_{i=0}^{n} \dfrac{\binom{k}{i}}{\binom{n}{i}} = \dfrac{\binom{n+1}{n-k+1}}{\binom{n}{k}}$
36. **Derangement:** a permutation of the elements of a set, such that no element appears in its original position. Let $d(n)$ be the number of derangements of the identity permutation fo size $n$.
    
    $$d(n)=(n-1) \cdot (d(n-1)+d(n-2)) \, \text{where}\;d(0)=1,d(1)=0$$
37. **Involutions:** permutations such that $\displaystyle p^2 =$ identity permutation. $\displaystyle a_0 = a_1 = 1$ and $\displaystyle a_n=a_{n-1} + (n-1)a_{n-2}$ for $n>1$.
38. Let $T(n,k)$ be the number of permutations of size $n$ for which all cycles have length $\displaystyle \leq k$.
    
    $$
        T(n, k)=
        \begin{cases} 
          n! & ; n \le k\\
          n \cdot T(n-1, k) - F(n-1, k) \cdot T(n-k-1, k) & ;n > k \\
       \end{cases}
    $$  
    Here $\displaystyle F(n, k) = n \cdot (n - 1) \cdot ... \cdot (n - k + 1)$
39. **Lucas Theorem**
     1. If $\displaystyle p$ is prime, then $\displaystyle \left(\frac{p^{a}}{k}\right) \equiv 0 (\mod\; p)$  
     2. For non-negative integers $m$ and $n$ and a prime $\displaystyle p$, the following congruence relation holds:
      
        $$\displaystyle \left(\frac{m}{n}\right) \equiv \prod_{i=0}^{k} \left(\frac{m_{i}}{n_{i}}\right) (mod\; p),$$
        where,  
        $m=m_{k} p^{k} +m_{k-1} p^{k-1}+...+m_{1} p+m_{0}$,  
        and   
        $n=n_{k}p^{k}+n_{k-1}p^{k-1}+...+n_{1}p+n_{0}$  
        are the base $\displaystyle p$ expansions of $m$ and $n$ respectively. This uses the convention that  $\displaystyle \left(\frac{m}{n}\right)=0$,when $m<n$.
40. $\displaystyle \sum_{i=0}^{n}  {n \choose i } \cdot i^{k}$  
    = $\displaystyle \sum_{i=0}^{n}  {n \choose i } \cdot \sum_{j=0}^{k}{ \left\\{ \begin{matrix} k\cr j \end{matrix} \right\\} \cdot i^{\underline{j}}}$  
    = $\displaystyle \sum_{i=0}^{n} {n \choose i } \cdot \sum_{j=0}^{k} \left\\{ \begin{matrix} k\cr j \end{matrix} \right\\} \cdot  j! {n \choose i }$  
    = $\displaystyle \sum_{i=0}^{n} \frac{n!}{(n-i)!} \cdot \sum_{j=0}^{k} \left\\{ \begin{matrix}k\cr j \end{matrix} \right\\} \cdot \frac{1}{(i-j)!}$  
    = $\displaystyle \sum_{i=0}^{n} \sum_{j=0}^{k} \frac{n!}{(n-i)!} \cdot  \left\\{\begin{matrix} k\cr j \end{matrix} \right\\} \cdot \frac{1}{(i-j)!}$  
    = n!$\displaystyle \sum_{i=0}^{n} \sum_{j=0}^{k} \left\\{ \begin{matrix} k\cr j \end{matrix} \right\\} \cdot \frac{1}{(n-i)!} \cdot \frac{1}{(i-j)!}$  
    = n!$\displaystyle \sum_{i=0}^{n} \sum_{j=0}^{k} \left\\{ \begin{matrix} k\cr j \end{matrix} \right\\} \cdot { n-j \choose n-i} \cdot \frac{1}{(n-j)!}$  
    = n!$\displaystyle \sum_{j=0}^{k} \left\\{ \begin{matrix} k\cr j \end{matrix} \right\\} \cdot \frac{1}{(n-j)!} \sum_{i=0}^{n} \cdot { n-j \choose n-i}$  
    = $\displaystyle \sum_{j=0}^{k} \left\\{\begin{matrix} k\cr j \end{matrix} \right\\} \cdot n^{\underline{j}} \cdot 2^{n-j}$
    
    Here $n^{\underline{j}}=P(n,j)=\dfrac{n!}{(n-j)!}$ and $\displaystyle \left\\{ \begin{matrix} k\cr j \end{matrix} \right\\}$ is stirling number of the second kind.
    
    So, instead of $O(n)$, now you can calculate the original equation in $O(k^2)$ or even in $O(k \log^2 n)$ using NTT.
41. $\displaystyle \displaystyle \sum \limits_{i=0}^{n-1} {i \choose j} x^i = x^j(1-x)^{-j-1}\left( 1- x^n \sum \limits_{i=0}^j {n \choose i} x^{j-i} (1-x)^i \right)$
42. $\displaystyle x_{0}, x_{1}, x_{2}, x_{3}, ... , x_{n}$  
    $\displaystyle x_{0} + x_{1}, x_{1} + x_{2}, x_{2}+x_{3}, ... x_{n}$  
    ...  
    If we continuously do this $n$ times then the polynomial of the first column of the $n$-th row will be
    
    $$\displaystyle p(n)=\sum_{k=0}^{n}{n \choose k} \cdot x(k)$$
43. If $\displaystyle P(n)=\sum_{k=0}^{n}{n \choose k} \cdot Q(k)$,
    then, 
    
    $$
    Q(n)=\sum_{k=0}^{n}(-1)^{n-k}{n \choose k} \cdot P(k) 
    $$
44. If $\displaystyle P(n)=\sum_{k=0}^{n}(-1)^{k}{n \choose k} \cdot Q(k)$ ,
    then, 
    
    $$
    Q(n)=\sum_{k=0}^{n}(-1)^{k}{n \choose k} \cdot P(k)
    $$
     
    #### Catalan Numbers
45. $\displaystyle C_n=\frac{1}{n+1}{2n \choose n}$
46. $\displaystyle C_0=1,C_1=1\text{ and }C_n=\sum \limits_{k=0}^{n-1}C_k C_{n-1-k}$
47. Number of correct bracket sequence consisting of $n$ opening and $n$ closing brackets.
48. The number of ways to completely parenthesize $n$+$\displaystyle 1$ factors.
49. The number of triangulations of a convex polygon with  $n$+$\displaystyle 2$ sides (i.e. the number of partitions of polygon into disjoint triangles by using the diagonals).
50. The number of ways to connect the $\displaystyle 2n$ points on a circle to form $n$ disjoint i.e. non-intersecting  chords.
51. The number of monotonic lattice paths from point $\displaystyle (0,0)$ to point $\displaystyle (n,n)$ in a square lattice of size $n\times n$, which do not pass above the main diagonal (i.e. connecting $\displaystyle (0,0)$ to $\displaystyle (n,n)$).
52. The number of rooted full binary trees with $n$+$\displaystyle 1$ leaves (vertices are not numbered). A rooted binary tree is full if every vertex has either two children or no children.
53. Number of permutations of $\displaystyle \{1, …, n\}$ that avoid the pattern $\displaystyle 123$ (or any of the other patterns of length $3$); that is, the number of permutations with no three-term increasing sub-sequence. For $n = 3$, these permutations are $\displaystyle 132,\ 213,\ 231,\ 312$ and $321.$\displaystyle For $n = 4$, they are $\displaystyle 1432,\ 2143,\ 2413,\ 2431,\ 3142,\ 3214,\ 3241,\ 3412,\ 3421,\ 4132,\ 4213,\ 4231,\ 4312$ and $4321.$
54. **Balanced Parentheses count with prefix:**
    The count of balanced parentheses sequences consisting of $n+k$ pairs of parentheses where the first $\displaystyle \displaystyle k$ symbols are open brackets. Let the number be $\displaystyle C_n^{(k)}$, then
    
    $$\displaystyle \displaystyle C_n^{(k)} = \frac{k+1}{n+k+1} \binom{2n+k}{n}$$
   
    #### Narayana numbers
55. $N(n,k)=\frac{1}{n}\left(\frac{n}{k}\right)\left(\frac{n}{k-1}\right)$
56. The number of expressions containing $n$ pairs of parentheses, which are correctly matched and which contain $\displaystyle \displaystyle k$ distinct nestings. For instance, $N(4, 2) = 6$ as with four pairs of parentheses six sequences can be created which each contain two times the sub-pattern '()'.

    #### Stirling numbers of the first kind
57. The Stirling numbers of the first kind count permutations according to their number of cycles (counting fixed points as cycles of length one).
58. $S(n,k)$ counts the number of permutations of $n$ elements with $\displaystyle \displaystyle k$ disjoint cycles.
59. $S(n,k)=(n-1) \cdot S(n-1,k)+S(n-1,k-1),$
    $$where,\; S(0,0)=1,S(n,0)=S(0,n)=0$$
60. $\displaystyle \displaystyle\sum_{k=0}^{n}S(n,k) = n!$
61. The unsigned Stirling numbers may also be defined algebraically, as the coefficient of the rising factorial:
    
    $$\displaystyle x^{\bar{n}} = x(x+1)...(x+n-1) = \sum_{k=0}^{n}{ S(n, k) x^k}$$
62. Lets $[n, k]$ be the stirling number of the first kind, then 
     
     $$\displaystyle \bigl[\!\begin{smallmatrix} n \\ n\ -\ k \end{smallmatrix}\!\bigr] = \sum_{0 \leq i_1 < i_2 < i_k < n}{i_1i_2....i_k.}$$

    #### Stirling numbers of the second kind
63. Stirling number of the second kind is the number of ways to partition a set of n objects into k non-empty subsets.
64. $S(n,k)=k \cdot S(n-1,k)+S(n-1,k-1)$,
    $$ where \; S(0,0)=1,S(n,0)=S(0,n)=0 $$
65. $S(n,2)=2^{n-1}-1$
66. $S(n,k) \cdot k!$ = number of ways to color $n$ nodes using colors from $\displaystyle 1$ to $\displaystyle \displaystyle k$ such that each color is used at least once.
67. An $r$-associated Stirling number of the second kind is the number of ways to partition a set of $n$ objects into $\displaystyle \displaystyle k$ subsets, with each subset containing at least $r$ elements. It is denoted by $S_r( n , k )$ and obeys the recurrence relation.
     $\displaystyle \displaystyle S_r(n+1,k) = k S_r(n,k) + \binom{n}{r-1} S_r(n-r+1,k-1)$
68. Denote the n objects to partition by the integers $\displaystyle 1, 2, ...., n$. Define the reduced Stirling numbers of the second kind, denoted $S^d(n, k)$, to be the number of ways to partition the integers $\displaystyle 1, 2, ...., n$ into k nonempty subsets such that all elements in each subset have pairwise distance at least d. 
     That is, for any integers i and j in a given subset, it is required that $|i - j| \geq d$. It has been shown that these numbers satisfy,
     $$S^d(n, k) = S(n - d + 1, k - d + 1), n \geq k \geq d$$

    #### Bell number
69. Counts the number of partitions of a set.
70. $B_{n+1}=\displaystyle\sum_{k=0}^{n}\left(\frac{n}{k}\right)*B_{k}$
71. $B_{n}=\displaystyle\sum_{k=0}^{n}S(n,k)$ ,where $S(n,k)$ is stirling number of second kind.

    ### Math
    #### General
72. $\displaystyle ab \mod\ ac=a(b \mod\ c)$
73. $\displaystyle \sum_{i = 0}^n{i\cdot i!=(n + 1)! - 1}$.
74. $\displaystyle a^k - b^k = (a - b) \cdot (a^{k - 1}b^0 + a^{k - 2}b^1 + ... + a^0b^{k - 1})$
75. $\displaystyle \min(a + b, c) = a + \min(b, c - a)$
76. $\|a - b\| + \|b - c\| + \|c - a\| = 2 (\max (a, b, c) - \min (a, b, c))$
77. $\displaystyle a \cdot b \leq c \rightarrow a \leq \left \lfloor \dfrac{c}{b} \right \rfloor$ is correct
78. $\displaystyle a \cdot b < c \rightarrow a <  \left \lfloor \dfrac{c}{b} \right \rfloor$ is incorrect
79. $\displaystyle a \cdot b \geq c \rightarrow a \geq  \left \lfloor \dfrac{c}{b} \right \rfloor$  is correct
80. $\displaystyle a \cdot b > c \rightarrow a >  \left \lfloor \dfrac{c}{b} \right \rfloor$ is correct
81. For positive integer $n$, and arbitrary real numbers $m,x$,
    
    $\displaystyle \left \lfloor \dfrac{\left \lfloor x/m \right \rfloor}{n} \right \rfloor = \left \lfloor \dfrac{x}{mn} \right \rfloor$
    
    $\displaystyle \left \lceil \dfrac{\left \lceil x/m \right \rceil}{n} \right \rceil = \left \lceil \dfrac{x}{mn} \right \rceil$
82. Lagrange's identity:
    
    $$\displaystyle \displaystyle {\displaystyle {\begin{aligned}\left(\sum \limits_{k=1}^{n}a_{k}^{2}\right)\left(\sum \limits_{k=1}^{n}b_{k}^{2}\right)-\left(\sum\limits_{k=1}^{n}a_{k}b_{k}\right)^{2}&=\sum \limits_{i=1}^{n-1}\sum \limits_{j=i+1}^{n}\left(a_{i}b_{j}-a_{j}b_{i}\right)^{2}\\&={\frac {1}{2}}\sum \limits_{i=1}^{n}\sum \limits_{j=1,j\neq i}^{n}(a_{i}b_{j}-a_{j}b_{i})^{2}\end{aligned}}}$$
    
83. $\displaystyle \sum_{i = 1}^n{ia^i} = \frac{a(n a^{n + 1} - (n + 1) a^n + 1)}{(a - 1)^2}$
84. **Vieta's formulas:**  
    Any general polynomial of degree $n$
    
    $$\displaystyle p(x) = a_nx^n + a_{n - 1}x^{n - 1} + ... + a_1x + a_0$$

    (with the coefficients being real or complex numbers and $\displaystyle a_n \neq 0$) is known by the fundamental theorem of algebra to have $n$ (not necessarily distinct) complex roots $r_1, r_2,..., r_n$.
    
    $$
        \begin{cases}
        \text{$r_1 + r_2 + ... + r_{n - 1} + r_n = - \frac{a_{n - 1}}{a_n}$}
        \\
        \text{$\displaystyle (r_1r_2 + r_1r_3 + ... + r_1r_n) + (r_2r_3 + r_2r_4 + ... + r_2r_n) + ... + r_{n - 1}r_n = \frac{a_{n - 2}}{a_n}$}
        \\\vdots\\
        \text{$r_1r_2...r_n = (-1)^n\frac{a_0}{a_n}.$}
        \end{cases}       
    $$  

    Vieta's formulas can equivalently be written as
    
    $$\displaystyle \sum_{1 \leq i_1 < i_2 < ...<i_k \leq n} \Bigg(\prod_{j = 1}^k{r_{i_j}}\Bigg) = (-1)^k\frac{a_{n - k}}{a_n},$$

85. We are given n numbers $\displaystyle a_1,a_2,...,a_n$ and our task is to find a value $\displaystyle x$ that minimizes the sum, 
    
    $$|a_1 - x| + |a_2 - x| + ... + |a_n - x|$$  

    optimal $\displaystyle x=$ median of the array.  
    if $n$ is even $\displaystyle x =$ $[$left median,right median$]$ i.e. every number in this range will work.

    For minimizing
    
    $$\displaystyle (a_1 - x)^2 + (a_2 - x)^2 + ... + (a_n - x)^2$$  

    optimal $\displaystyle x = \dfrac{(a_1 + a_2 + ... + a_n)}{ n}$
86. Given an array a of n non-negative integers. The task is to find the sum of the product of elements of all the possible subsets. It is equal to the product of $\displaystyle (a_i + 1)$ for all $\displaystyle a_i$
87. **Pentagonal number theorem:**
     In mathematics, the pentagonal number theorem states that
    
     $$\displaystyle \prod_{n = 1}^{\infty}\left ( 1 - x^n \right ) = \prod_{k = -\infty}^{\infty} \left ( -1 \right )^kx^{\frac{k(3k - 1)}{2}} = 1 + \prod_{k = 1}^{\infty}\left (-1\right )^k\left ( x^{\frac{k(3k + 1)}{2}} + x^{\frac{k(3k - 1)}{2}}\right ).$$   

     In other words, 
    
     $$\displaystyle (1 - x)(1 - x ^ 2)(1 - x^3)\cdots =1 - x - x^2 + x^5 + x^7 - x^{12} - x^{15} + x^{22} + x^{26} - \cdots.$$

     The exponents $\displaystyle 1, 2, 5, 7, 12,\cdots$ on the right hand side are given by the formula $g_k = \frac{k(3k - 1)}{2}$ for $\displaystyle \displaystyle k = 1, -1, 2, -2, 3, \cdots$ and are called (generalized) pentagonal numbers.  


     It is useful to find the [partition number](https://en.wikipedia.org/wiki/Partition_(number_theory)) in $O(n \sqrt{n})$


    #### Fibonacci Number
88. $\displaystyle F_0=0, F_1=1$ and $\displaystyle F_n=F_{n-1}+F_{n-2}$
89. $\displaystyle F_n=\sum\limits_{k=0}^{\lfloor\frac{n-1}{2}\rfloor}\binom{n-k-1}{k}$
90. $\displaystyle F_n=\frac{1}{\sqrt{5}}(\frac{1+\sqrt{5}}{2})^n-\frac{1}{\sqrt{5}}(\frac{1-\sqrt{5}}{2})^n$
91. $\displaystyle \sum\limits_{i=1}^{n}F_i=F_{n+2}-1$
92. $\displaystyle \sum\limits_{i=0}^{n-1}F_{2i+1}=F_{2n}$
93. $\displaystyle \sum\limits_{i=1}^{n}F_{2i}=F_{2n+1}-1$
94. $\displaystyle \sum\limits_{i=1}^{n}F_{i}^{2}=F_nF_{n+1}$
95. $\displaystyle F_mF_{n+1}-F_{m-1}F_{n}=(-1)^nF_{m-n}$  
    $\displaystyle F_{2n}=F_{n+1}^2-F_{n-1}^2=F_n(F_{n+1}+F_{n-1})$
96. $\displaystyle F_mF_n+F_{m-1}F_{n-1}=F_{m+n-1}$  
    $\displaystyle F_mF_{n+1}+F_{m-1}F_{n}=F_{m+n}$
97. A number is Fibonacci if and only if one or both of $\displaystyle (5 \cdot n^2 + 4)$ or $\displaystyle (5 \cdot n^2 - 4)$ is a perfect square
98. Every third number of the sequence is even and more generally, every $\displaystyle \displaystyle k^{th}$ number of the sequence is a multiple of $\displaystyle F_k$
99.  $gcd(F_m, F_n)=F_{gcd(m, n)}$
100. Any three consecutive Fibonacci numbers are pairwise coprime, which means that, for every n, $gcd(F_n, F_{n+1})=gcd(F_n, F_{n+2}), gcd(F_{n+1}, F_{n+2})=1$
101. If the members of the Fibonacci sequence are taken $mod$ $n$, the resulting sequence is periodic with period at most $6n$.
    
     #### Pythagorean Triples
102. A Pythagorean triple consists of three positive integers $\displaystyle a, b,$ and $\displaystyle C$, such that $\displaystyle a^{2}+b^{2}=c^{2}$. Such a triple is commonly written $\displaystyle (a, b, c)$
103. Euclid's formula is a fundamental formula for generating Pythagorean triples given an arbitrary pair of integers m and n with $m >n >0$. The formula states that the integers  
     
     $$\displaystyle a = m^{2}-n^{2}, b = 2mn,  c = m^{2}+n^{2}$$    
     
     form a Pythagorean triple. The triple generated by Euclid's formula is primitive if and only if m and n are coprime and not both odd. When both m and n are odd, then a, b, and c will be even, and the triple will not be primitive; however, dividing a, b, and c by 2 will yield a primitive triple when m and n  are coprime and both odd.
104. The following will generate all Pythagorean triples uniquely:  
     
     $$\displaystyle a = k\cdot \left( m^{2}-n^{2}\right), b = k\cdot\left(2mn\right),  c = k\cdot \left(m^{2}+n^{2}\right)$$  

     where m, n, and k are positive integers with $m > n$, and with m and n coprime and not both odd.  
105. **Theorem:**
     The number of Pythagorean triples
     {a,b,n} with $max\{a,b,n\} = n$ is given by  

     $$\displaystyle \dfrac{1}{2}\left( \displaystyle\prod _{ p^{\alpha} || n}\left( 2\alpha +1\right) -1\right)$$  

     where the product is over all prime divisors p of the form $4k+1$.  
     The notation $\displaystyle p^{\alpha} || n$ stands for the highest exponent $\displaystyle \alpha$ for which $\displaystyle p^{\alpha}$ divides $n$  
     **Example:**
     For $n = 2\cdot3^{2}\cdot5^{3}\cdot7^{4}\cdot11^{5}\cdot13^{6},$ the number of Pythagorean triples with hypotenuse n is $\displaystyle \dfrac{1}{2}\left( 7.13-1\right) =45$.  
     To obtain a formula for the number of Pythagorean triples with hypotenuse less than a specific positive integer N, we may add the numbers corresponding to each $n < N$ given by the Theorem. There is no simple way to compute this as a function of N.

     #### Sum of Squares Function
106. The function is defined as  
     $r_{k}\left(n\right) = \left|\{\left(a_{1},a_{2},...,a_{k} \right) \in \mathbf{Z^{k}} : n=a_{1}^{2}+a_{2}^{2}+...+a_{k}^{2}\}\right|$  
107.   The number of ways to write a natural number as sum of two squares is given by $r_2(n)$. It is given explicitly by  
    $r_{2}\left(n\right) = 4\left(d_{1}\left(n\right) - d_{3}\left(n\right)\right)$ 
    where d1(n) is the number of divisors of n which are congruent with 1 modulo 4 and d3(n) is the number of divisors of n which are congruent with 3 modulo 4.  <br> <br>
    The prime factorization $n = 2^{g}p_{1}^{f_{1}}p_{2}^{f_{2}}. . .q_{1}^{h_{1}}q_{2}^{h_{2}}. . . ,$  where $\displaystyle p_{i}$ are the prime factors of the form $\displaystyle p_{i} \equiv 1$ (mod 4), and $q_{i}$ are the prime factors of the form $q_{i} \equiv 3$ (mod 4) gives another formula   $r_{2}\left(n\right) = 4\left(f_{1}+1\right)\left(f_{2}+1\right)...,$ if all exponents $h_{1}$,$h_{2}$,... are even. If one or more $h_{i}$ are odd, then $r_{2}\left(n\right) = 0.$  
108. The number of ways to represent n as the sum of four squares is eight times the sum of all its divisors which are not divisible by 4, i.e.  
     $r_{4}\left( n \right) = 8 \displaystyle\sum _{d| n;4 \nmid d}d$    
     $r_{8}\left(n\right) = 16 \displaystyle\sum _{d|n} \left(-1\right)^{n+d}d^{3}$    

     ### Number Theory
     #### General
109. for $i > j$, $\displaystyle \gcd(i, j)$ $ = $ $\displaystyle \gcd(i -j, j)$ $\displaystyle \leq (i -j)$
110. $\displaystyle \sum_{x = 1}^n \left[ d \| x^k \right] = \left \lfloor\dfrac{n}{\prod_{i = 0}{p_i^{\left \lceil \dfrac{e_i}{k}\right \rceil}}}\right \rfloor$, 
     
     where $d = \prod_{i = 0}{p_i^{e_i}}$. Here, $[a \| b]$ means if $\displaystyle a$ divides $b$ then it is $\displaystyle 1$, otherwise it is $0$.
111. The number of lattice points on segment $\displaystyle (x_1,y_1)$ to $\displaystyle (x_2,y_2)$ is $\displaystyle \gcd(abs(x_1-x_2),abs(y_1-y_2)) + 1$
112. $\displaystyle (n-1)! \mod  n = n -1$ if n is prime, 2 if $n = 4$, $0$ otherwise.
113. A number has odd number of divisors if it is  perfect square
114. The sum of all divisors of a natural number n is odd if and only if $n=2^r\cdot k^2$ where $r$ is non-negative and $\displaystyle \displaystyle k$ is positive integer.
115. Let $\displaystyle a$ and $b$ be coprime positive integers, and find integers $\displaystyle a{\prime}$ and $b{\prime}$ such that $\displaystyle aa{\prime} \equiv 1 \mod b$ and $bb{\prime} \equiv 1 \mod a$. Then the number of representations of a positive integers \(n\) as a non negative linear combination of $\displaystyle a$ and $b$ is  
     
     $$\displaystyle \frac{n}{ab}-\Big\{\frac{b{\prime} n}{a}\Big\}-\Big\{\frac{a{\prime} n}{b}\Big\} + 1$$

     Here, $\displaystyle \{x\}$ denotes the fractional part of $\displaystyle x$.
116. $$\displaystyle \displaystyle \sum \limits_{i=1}^{a}\sum \limits_{j=1}^{b}\sum \limits_{k=1}^{c} d(i \cdot j \cdot k) = \sum \limits_{\gcd (i,j)=\gcd (j,k) = \gcd (k,i) =1} \left \lfloor \dfrac{a}{i}\right \rfloor \left \lfloor \dfrac{b}{j}\right \rfloor \left \lfloor \dfrac{c}{k} \right \rfloor$$
       
     Here, $d(x) =$ number of divisors of $\displaystyle x$.
117. **Gauss's generalization of Wilson's theorem:**,  
     Gauss proved that,  
     
     $$\displaystyle \displaystyle \prod \limits_{k=1 \atop \gcd(k,m)=1}^{m}\!\!k\ \equiv {\begin{cases}-1{\pmod {m}}&{\text{if }}m=4,\;p^{\alpha },\;2p^{\alpha }\\\;\;\,1{\pmod {m}}&{\text{otherwise}}\end{cases}}$$

     where $\displaystyle p$ represents an odd prime and $\displaystyle \alpha$  a positive integer. The values of $m$ for which the product is $-1$ are precisely the ones where there is a primitive root modulo $m$.

     #### Divisor Function
118. $\displaystyle \sigma_x(n)=\sum\limits_{d\vert n}^{}d^x$
119. It is multiplicative i.e if $\displaystyle \gcd(a, b)=1\to \sigma_x(ab)=\sigma_x(a)\sigma_x(b)$.
120. $$\displaystyle \sigma_x(n)=\prod\limits_{i=1}^{\tau}\frac{p_i^{(a_i+1)x}-1}{p_i^x-1}$$
121. **Divisor Summatory Function**
     1. Let $\displaystyle \sigma_0(k)$ be the number of divisors of $\displaystyle \displaystyle k$.
     2. $D(x)=\sum\limits_{n\leq{x}}{\sigma_0(n)}$
     3. $D(x)=\sum\limits_{k=1}^{x}\lfloor\frac{x}{k}\rfloor=2\sum\limits_{k=1}^{u}\lfloor\frac{x}{k}\rfloor-u^2$, where $u=\sqrt{x}$
     4. $D(n)=$Number of increasing arithmetic progressions where $n+1$ is the second or later term. (i.e. The last term, starting term can be any positive integer $\displaystyle \le n$. For example, $D(3)=5$ and there are 5 such arithmetic progressions: $\displaystyle (1, 2, 3, 4); (2, 3, 4); (1, 4); (2, 4); (3, 4).$
122. Let $\displaystyle \sigma_1(k)$ be the sum of divisors of k. Then, $\displaystyle \sum\limits_{k=1}^{n}\sigma_1(k)=\sum\limits_{k=1}^{n}{k \left\lfloor \frac{n}{k} \right\rfloor}$
123. $\displaystyle \prod\limits_{d\vert n}^{}d={n^{\frac{\sigma_0}{2}}}$ if $n$ is not a perfect square, and $=\sqrt{n} \cdot n^{\frac{\sigma_0-1}{2}}$ if $n $ is a perfect square.
     #### Euler’s Totient function
124. The function is multiplicative.  
  This means that if $\displaystyle \gcd(m, n) = 1$, $\displaystyle \phi(m \cdot n) = \phi(m) \cdot \phi(n)$.
125. $\displaystyle \phi(n) = n\prod_{p \|n}(1 - \frac{1}{p} )$
126. If p is prime and \(k \geq 1\), then, 
  $\displaystyle \phi(p^k) = p^{k - 1}(p - 1) = p^k(1 - \frac{1}{p})$
127. $J_k(n)$, the Jordan totient function, is the number of $\displaystyle \displaystyle k$-tuples of positive integers all less than or equal to n that form a coprime $\displaystyle (k + 1)$-tuple together with $n$. It is a generalization of Euler's totient, $\displaystyle \phi(n) = J_1(n)$.    
     $$J_k(n) = n^k\prod_{p |n}(1 - \frac{1}{p^k})$$
128. $\displaystyle \sum_{d\|n}J_k(d) = n^k$
129. $\displaystyle \sum_{d\|n}\phi(d) = n$
130. $\displaystyle \phi(n) = \sum_{d\|n}\mu(d)\cdot\frac{n}{d} = n\sum_{d\|n}\frac{\mu(d)}{d}$
131. $\displaystyle \phi(n) = \sum_{d\|n}d\cdot\mu(\frac{n}{d})$
 
132. $\displaystyle \displaystyle {a}\vert{b} \to \varphi(a)\vert{\varphi(b)}$
133. $n\vert{\varphi(a^n - 1)}$ for $\displaystyle a, n > 1$    
134. $\displaystyle \varphi(mn)=\varphi(m)\varphi(n)\cdot\frac{d}{\varphi(d)}$ where $d=gcd(m, n)$  
     Note the special cases
     
     $$
        \varphi(2m)=
        \begin{cases} 
          2\varphi(m) & ; if \, m  \, is \, even\\
          \varphi(m) & ; if \, m \, is \, odd\\
        \end{cases}$$  
     
     $$\displaystyle \varphi(n^m)=n^{m-1}\varphi(n)$$

135. $\displaystyle \varphi(lcm(m, n)) \cdot \varphi(gcd(m, n))=\varphi(m) \cdot \varphi(n)$  
  Compare this to the formula $lcm(m, n)\cdot gcd(m,n)=m\cdot n$
136. $\displaystyle \varphi(n)$ is even for $n\geq3$. Moreover, if if $n$ has $r$ distinct odd prime factors, $\displaystyle 2^r \vert \varphi(n)$
137. $\displaystyle \sum\limits_{d\vert{n}}^{} \frac{\mu^2(d)}{\varphi(d)}=\frac{n}{\varphi(n)}$
138. $\displaystyle \sum\limits_{1\leq k \leq n, \gcd(k, n)=1}k=\frac{1}{2}n\varphi(n)$ for $n > 1$
139. $\displaystyle \frac{\varphi(n)}{n}=\frac{\varphi(rad(n))}{rad(n)}$ where $rad(n)=$ 
    $\displaystyle \prod\limits_{p\vert n, p \, prime} p$
140. $\displaystyle \lfloor\frac{n}{\varphi(n)}\rfloor$ is periodic. $\displaystyle 1, 2, 1, 2, 1, 3, 1, 2, 1, 2, 1, 3, ...$
141. $\displaystyle \phi(m) \geq \log_2{m}$
142. $\displaystyle \phi(\phi(m))\leq\frac{m}{2}$
143. When $\displaystyle x \geq \log_2m$, then 
     
     $$n^x\mod m=n^{\phi(m) + x\mod \phi(m)}\mod m$$
144. $\displaystyle \sum\limits_{1\leq k\leq n, \gcd(k, n)=1}\gcd(k-1, n)=\varphi(n)d(n)$ where $d(n)$ is number of divisors. Same equation for $\displaystyle \gcd(a \cdot k-1, n)$ where $\displaystyle a$ and $n$ are coprime.
145. For every $n$ there is at least one other integer $m\ne n$ such that $\displaystyle \varphi(m)=\varphi(n).$
146. $\displaystyle \sum\limits_{i=1}^{n} {\varphi(i) \cdot \lfloor\frac{n}{i}\rfloor=\frac{n*(n+1)}{2}}$
147. $\displaystyle \sum\limits_{i=1, i \% 2 \ne 0 }^{n} \varphi(i) \cdot \lfloor\frac{n}{i}\rfloor=\sum\limits_{k\geq 1}[\frac{n}{2^k}]^2$.
  Note that $[\, ]$ is used here to denote round operator not floor or ceil
148. $$\displaystyle \sum\limits_{i=1}^{n}\sum\limits_{j=1}^{n}ij[\gcd(i, j)=1]=\sum\limits_{i=1}^{n}\varphi(i)i^2$$
149. Average of coprimes of $n$ which are less than $n$ is $\displaystyle \dfrac{n}{2}$.
     #### Mobius Function and Inversion
150. For any positive integer $n$, define $\displaystyle \mu(n)$ as the sum of the primitive $n^{th}$ roots of unity. It has values in $\displaystyle \{-1, 0, 1\}$ depending on the factorization of $n$ into prime factors: 
     1. $\displaystyle \mu(n)=1$ if $n$ is a square-free positive integer with an even number of prime factors.
     2. $\displaystyle \mu(n)=-1$ if $n$ is a square-free positive integer with an odd number of prime factors.
     3. $\displaystyle \mu(n)=0$ if $n$ has a squared prime factor.
151. It is a multiplicative function.
152. $$ 
        \sum_{d|n}\mu(d) =
        \begin{cases} 
          1 & ; n=1\\
          0 & ; n > 0
       \end{cases}$$
153. $\displaystyle \displaystyle \sum\limits_{n=1}^N {\mu}^2(n) = \displaystyle \sum\limits_{n=1}^{\sqrt{N}} \mu(k) \cdot \left \lfloor \dfrac{N}{k^2} \right\rfloor$
     This is also the number of square-free numbers $\displaystyle \le n$ 
154. **Mobius inversion theorem:** The classic version states that if g and f are arithmetic functions satisfying
    $g(n) = \displaystyle \sum_{d|n}f(d) $ for every integer $n \ge 1$ then $g(n) = \displaystyle \sum_{d|n}\mu(d)g\left(\frac{n}{d}\right)$ for every integer $n \ge 1$
155. If $\displaystyle F(n) = \displaystyle \prod_{d\|n} f(d)$, then $\displaystyle F(n) = \displaystyle \prod_{d\|n} F\left(\frac{n}{d}\right)^{\mu(d)}$
156. $\displaystyle \displaystyle \sum_{d|n}\mu(d)\phi(d) = \displaystyle \prod_{j=1}^K (2 - P_j)$
    where $\displaystyle p_j$  is the primes factorization of $d$  
157. If $\displaystyle F(n)$ is multiplicative, $\displaystyle F \not\equiv 0$, then $\displaystyle \displaystyle \sum_{d|n} \mu(d) f(d) = \displaystyle \prod_{i=1} (1 - f(P_i)) \cdot$
    where $\displaystyle p_i$  are primes of $n$.

     #### GCD and LCM
158. $\displaystyle \gcd(a, 0) = a$
159. $\displaystyle \gcd(a, b) = \gcd(b, a \mod b)$
160. Every common divisor of $\displaystyle a$ and $b$ is a divisor of $\displaystyle \gcd(a,b)$.
161. if $m$ is any integer, then $\displaystyle \gcd(a + m {\cdot} b, b) = \gcd(a, b)$
162. The gcd is a multiplicative function in the following sense: if $\displaystyle a_1$ and $\displaystyle a_2$ are relatively prime, then $\displaystyle \gcd(a_1 \cdot a_2, b) = \gcd(a_1, b) \cdot \gcd(a_2,b )$.
163. $\displaystyle \gcd(a, b){\cdot} \operatorname{lcm}(a, b) = \|a{\cdot}b\|$
164. $\displaystyle \gcd(a, \operatorname{lcm}(b, c)) = \operatorname{lcm}(\gcd(a, b), \gcd(a, c))$.
165. $\displaystyle \operatorname{lcm}(a, \gcd(b, c)) = \gcd(\operatorname{lcm}(a, b), \operatorname{lcm}(a, c))$.
166. For non-negative integers $\displaystyle a$ and $b$, where $\displaystyle a$ and $b$ are not both zero, $\displaystyle \gcd({n^a} - 1, {n^b} - 1) = n^{\gcd(a,b)} - 1$
167. $\displaystyle \gcd(a, b) = \displaystyle \sum_{k\|a \, \text{and} \, k\|b} {\phi(k)}$  
168. $\displaystyle \displaystyle \sum_{i=1}^n [\gcd(i, n) = k] = { \phi{\left(\frac{n}{k}\right)}}$
169. $\displaystyle \displaystyle \sum_{k=1}^n \gcd(k, n) = \displaystyle \sum_{d\|n} d \cdot {\phi{\left(\frac{n}{d}\right)}}$
170. $\displaystyle \displaystyle \sum_{k=1}^n x^{\gcd(k,n)} = \displaystyle \sum_{d\|n} x^d \cdot {\phi{\left(\frac{n}{d}\right)}}$
171. $\displaystyle \displaystyle \sum_{k=1}^n \frac{1}{\gcd(k, n)} = \displaystyle \sum_{d\|n} \frac{1}{d} \cdot {\phi{\left(\frac{n}{d}\right)}} = \frac{1}{n} \displaystyle \sum_{d\|n} d \cdot \phi(d)$
172. $\displaystyle \displaystyle \sum_{k=1}^n \frac{k}{\gcd(k, n)} = \frac{n}{2} \cdot \displaystyle \sum_{d\|n} \frac{1}{d} \cdot {\phi{\left(\frac{n}{d}\right)}} = \frac{n}{2} \cdot \frac{1}{n} \cdot \displaystyle \sum_{d\|n} d \cdot \phi(d)$
173. $\displaystyle \displaystyle \sum_{k=1}^n \frac{n}{\gcd(k, n)} = 2 * \displaystyle \sum_{k=1}^n \frac{k}{\gcd(k, n)} - 1$,  for  $n > 1$
174. $\displaystyle \displaystyle \sum_{i=1}^n \sum_{j=1}^n [\gcd(i, j) = 1] = \displaystyle \sum_{d=1}^n \mu(d) \lfloor {\frac{n}{d} \rfloor}^2$
175. $\displaystyle \displaystyle \sum_{i=1}^n \displaystyle\sum_{j=1}^n \gcd(i, j) = \displaystyle \sum_{d=1}^n \phi(d) \lfloor {\frac{n}{d} \rfloor}^2$
176. $\displaystyle \sum_{i=1}^n \sum_{j=1}^n i \cdot j[\gcd(i, j) = 1] = \sum_{i=1}^n \phi(i)i^2$
177. $\displaystyle F(n) = \displaystyle \sum_{i=1}^n \displaystyle \sum_{j=1}^n \operatorname{lcm}(i, j) = \displaystyle \sum_{l=1}^n {\left(\frac{\left( 1 + \lfloor{\frac{n}{l} \rfloor} \right) \left( \lfloor{\frac{n}{l} \rfloor} \right)} {2} \right)}^2 \displaystyle \sum_{d\|l} \mu(d)ld$
178. $\displaystyle \gcd(\operatorname{lcm}(a, b), \operatorname{lcm}(b, c), \operatorname{lcm}(a, c)) = \operatorname{lcm}(\gcd(a, b), \gcd(b, c), \gcd(a, c))$
179. $\displaystyle \gcd(A_L, A_{L+1}, ..., A_R) = \gcd(A_L, A_{L+1} - A_L, ..., A_R - A_{R-1})$.'
180. Given n, If $SUM = LCM(1,n) + LCM(2,n) + ... + LCM(n,n)$  
     then SUM = $\displaystyle \dfrac{n}{2}( \displaystyle\sum _{ d| n}\left( \phi \left( d\right) \times d\right) +1$
     #### Legendre Symbol
181. Let $\displaystyle p$ be an odd prime number. An integer $\displaystyle a$ is a quadratic residue modulo $\displaystyle p$ if it is congruent to a perfect square modulo $\displaystyle p$ and is a quadratic nonresidue modulo $\displaystyle p$ otherwise. The Legendre symbol is a function of $\displaystyle a$ and $\displaystyle p$ defined as
     
     $$\displaystyle \displaystyle \left( \frac{a}{p} \right)=
        {\begin{cases}
        \,1&{\text{if }}a\ {\text{is a quadatric residue modulo }}p\ {\text{and }}\ a\ \not\equiv\ 0 {\pmod{p}},\\\;\;\,-1&{\text{if }}a\ {\text{is a non-quadaratic residue modulo }}p,\\\;\;\,0&{\text{if }}a \equiv\ 0 {\pmod{p}}
        \end{cases}}$$
    
182. Legenres's original definition was by means of explicit formula  
     $\displaystyle \left(\frac{a}{p}\right)\equiv a^{\frac{p-1}{2}} \pmod{p} \ and \ \left(\frac{a}{p}\right)\in\{-1,0,1\}.$
    
183. The Legendre symbol is periodic in its first (or top) argument: if\ $\displaystyle a \equiv b \pmod{p}$, then  
     $\displaystyle \displaystyle \left(\frac{a}{p}\right)=\left(\frac{b}{p}\right).$
    
184. The Legendre symbol is a completely multiplicative function of its top argument:  
     $\displaystyle \displaystyle \left(\frac{ab}{p} \right) = \left(\frac{a}{p} \right) \left(\frac{b}{p} \right)$
    
185. The Fibonacci numbers $\displaystyle 1,1,2,3,5,8,13,21,34,55,...$ are defined by the recurrence $\displaystyle F_1 = F_2 = 1,F_{n+1} = F_n + F_{n-1}.$ If $\displaystyle p$ is a prime number then    
     $\displaystyle \displaystyle F_{p-\left(\frac{p}{5}\right)} \equiv 0 {\pmod{p}}, \;\;F_p \equiv \left(\frac{p}{5}\right) {\pmod{p}}.$

     For example,  
     $\displaystyle \displaystyle\left(\frac{2}{5}\right)=-1,\;\;\;F_3=2,\;\;\;F_2=1,$  
     $\displaystyle \displaystyle\left(\frac{3}{5}\right)=-1,\;\;\; F_4=3,\;\;\;F_3=2,$  
    
     $\displaystyle \displaystyle\left(\frac{5}{5}\right)=\;\;\;0,\;\;\; F_5=5,$
    
     $\displaystyle \displaystyle\left(\frac{7}{5}\right)=-1,\;\; F_8=21,\;\;F_7=13,$
     
     $\displaystyle \displaystyle\left(\frac{11}{5}\right)=\;\;1,\;\; F_{10}=55,\;\;F_{11}=89,$
    
186. Continuing from previous point, $\displaystyle \displaystyle \left(\frac{p}{5}\right)={\text{infinite concatenation of the sequence}}\left(1,-1,-1,1,0\right) {\text{from }}p \geq 1$.
187. If $n$ = $\displaystyle \displaystyle k^2$ is perfect square then $\displaystyle \left(\frac{n}{p}\right)=1$ for every odd prime except $\displaystyle \left(\frac{n}{k}\right)=0$ if k is an odd prime.  

     ### Miscellaneous
188. $\displaystyle \displaystyle a+b = a \oplus b +2(a \& b)$.
189. $\displaystyle \displaystyle a + b = a \mid b + a \& b$ 
190. $\displaystyle \displaystyle a \oplus b = a\mid b - a \& b$
191. $\displaystyle \displaystyle k_{th}$ bit is set in $\displaystyle x$ iff $\displaystyle x \mod 2^{k - 1}\geq 2^k$. It comes handy when you need to look at the bits of the numbers which are pair sums or subset sums etc.
192. $\displaystyle \displaystyle k_{th}$ bit is set in $\displaystyle x$ iff $\displaystyle x \mod 2^{k - 1} - x \mod 2^k \neq\ 0$ ($ = 2^k$ to be exact). It comes handy when you need to look at the bits of the numbers which are pair sums or subset sums etc.
193. $n \mod 2^i = n \& (2^i - 1)$
194. $\displaystyle 1\oplus 2 \oplus 3 \oplus \cdots \oplus (4k - 1) = 0$ for any $\displaystyle \displaystyle k \ge 0$
195. **Erdos Gallai Theorem:** 
     The degree sequence of an undirected graph is the non-increasing sequence of its vertex degrees  
     A sequence of non-negative integers $d_1 \geq d_2 \geq \cdots \geq d_n$ can be represented as the degree sequence of finite simple graph on $n$ vertices if and only if $d_1 + d_2 + \cdots + d_n$ is even and 
     
     $$\displaystyle \sum_{i = 1}^k {d_i \leq k(k - 1)} + \sum_{i = k + 1}^n \min(d_i, k)$$

     holds for every $\displaystyle \displaystyle k$ in $\displaystyle 1 \leq k \leq n$.

### Outro
A good life is just a series of good days. So make sure to have a good day, friend <a href="https://emoji.gg/emoji/8771_blobheart"><img src="https://emoji.gg/assets/emoji/8771_blobheart.png" width="16px" height="16px" alt="blobheart"></a>.

<iframe src="https://www.facebook.com/plugins/like.php?href=https%3A%2F%2Fshahjalalshohag.github.io%2Fnirvana%2F&width=450&layout=standard&action=like&size=small&share=true&height=35&appId" width="450" height="35" style="border:none;overflow:hidden" scrolling="no" frameborder="0" allowfullscreen="true" allow="autoplay; clipboard-write; encrypted-media; picture-in-picture; web-share"></iframe>

<div id="fb-root"></div>
<script async defer crossorigin="anonymous" src="https://connect.facebook.net/en_US/sdk.js#xfbml=1&version=v12.0" nonce="my6ulbt3"></script>

<div class="fb-comments" data-href="https://shahjalalshohag.github.io/equation-list/" data-width="" data-numposts="5"></div>