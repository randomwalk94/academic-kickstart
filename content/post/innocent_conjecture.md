+++
title = "A Conjecture on Linear Combinations of Rademacher Random Variables"

date = 2018-05-18
draft = false

tags = ["conjecture", "combinatorics", "probability theory"]
summary = "A seemingly innocent unsolved problem on the sum of Rademacher random variables (taking values $+ 1$ and $-1$ with equal probability $\\frac{1}{2}$)"

[header]
image = ""
caption = ""

+++
We note that the above holds if it holds for a subsequence `$n_k$`,
`\[{\bf{P}}[{S_{n_k}} > (1 - \varepsilon ){L_{n_k}},\;{\text{infinitely often}}] = 1.\]`
Pick an integer $N$ large enough (which we will specify later). Let `$n_k=N^k$`, `$\Delta n_k = n_k-n_{k-1}$`, and
`\[{A_k} = \left\{ {{S_{{n_k}}} - {S_{{n_{k - 1}}}} > \sqrt {2\Delta {n_k}\log \log{n_k}} \;} \right\}.\]`
The events $A_k$'s are independent. Moreover, we have that, for $k$ large enough, 
`\[\begin{aligned}
{\bf{P}}[{A_k}] &= {\bf{P}}[{S_{{n_k}}} - {S_{{n_{k - 1}}}} > \sqrt {2\Delta {n_k}\log \log {n_k}} ]\\
 &= {\bf{P}}\left[ {\frac{{{S_{{n_k}}} - {S_{{n_{k - 1}}}}}}{{\sqrt {\Delta {n_k}} }} > \sqrt {2\log \log{n_k}} } \right]\\
 &\ge \frac{C}{{\sqrt {2\log \log{n_k}} }}{e^{ - \log \log {n_k}}}\\
 &= \frac{{C'}}{{\sqrt {\log k + \log \log N} }} \cdot \frac{1}{k},
\end{aligned}\]`
We can see that the series `$\sum {\frac{1}{{k\sqrt {\log k} }}}  \approx \int {\frac{1}{{k\sqrt {\log k} }}}  = {(\log k)^{1/2}}$` diverges. Hence, `$\sum {{\bf{P}}[{A_k}]}  = \infty $`. By Borel-Cantelli, we get that `${\bf{P}}[{A_k},\;\text{infinitely often}] =1$`. More explicitly, there exists a set `$A$` of full measure so that for $\omega \in A$ we have
`\[{S_{{n_k}}} - {S_{{n_{k - 1}}}} > \sqrt {2\Delta {n_k}\log \log {n_k}} \]`
for infinitely many $k$. From (i), by replacing $X_i$ with $-X_i$ and letting $\E =1$, we can get a lower bound on $S_n$, which is
`\[{S_n}>  - 2\sqrt {2n\log \log n} \quad \text{for large enough $n$ a.s.}\]`
Overall, for $\omega \in A$, for infinitely many values of $k$, we get
`\[\begin{aligned}
{S_{{n_k}}}(\omega ) &= {S_{{n_{k - 1}}}}(\omega ) + \left( {{S_{{n_k}}} - {S_{{n_{k - 1}}}}} \right)(\omega )\\
 &\ge  - 2\sqrt {2{n_{k - 1}}\log \log {n_{k - 1}}}  + \sqrt {2\Delta {n_k}\log \log {n_k}} \\
 &=  - \frac{2}{{\sqrt N }}\sqrt {2{n_k}\log \log n_k}  + \sqrt {1 - \frac{1}{N}} \sqrt {2{n_k}\log \log n_k} .
\end{aligned}\]`
Choosing $N$ large enough so that `$\sqrt {1 - \frac{1}{N}}  > \frac{2}{{\sqrt N }} + 1 -\varepsilon$`, we will get the desired result.