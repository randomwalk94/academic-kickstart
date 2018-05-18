+++
title = "A Random Walk to Stochastic Analysis"

date = 2018-05-15
draft = false
highlight = true
tags = ["research", "probability theory", "stochastic processes","kpz universality"]
summary = "Notes and references to study stochastic calculus."

[header]
image = "/financial_stock.jpg"
caption = "Image credit: [**BACKGROUNDS4K**](http://backgrounds4k.net/stocks/)"

+++

Stochastic calculus is dedicated to the theory of _stochastic processes_. Just like classical calculus being the study of functions, stochastic calculus provides tools to operate on stochastic processes, which are in essence _random functions_.

We can see that the series `$\sum {\frac{1}{{k\sqrt {\log k} }}}  \approx \int {\frac{1}{{k\sqrt {\log k} }}}  = {(\log k)^{1/2}}$` diverges. Hence, $\sum {{\bf{P}}[{A_k}]}  = \infty $. By Borel-Cantelli, we get that ${\bf{P}}[{A_k},\;\text{infinitely often}] =1$. More explicitly, there exists a set $A$ of full measure so that for $\omega \in A$ we have
`\[\begin{aligned}
{\bf{P}}[{S_{{\left\lfloor {{n_{k + 1}}} \right\rfloor }}} > (1 + \varepsilon ){L_{{n_k}}}]& = {\bf{P}}\left[ {\frac{{{S_{{\left\lfloor {{n_{k + 1}}} \right\rfloor }}}}}{{\sqrt {{\left\lfloor {{n_{k + 1}}} \right\rfloor }} }} > (1 + \varepsilon )\frac{{\sqrt {2{n_k}\log \log {n_k}} }}{{\sqrt {{\left\lfloor {{n_{k + 1}}} \right\rfloor }} }}} \right] \\&\le C\exp \left[ { - \frac{1}{2}{{(1 + \varepsilon )}^2}\frac{{2{n_k}\log \log {n_k}}}{{{\left\lfloor {{n_{k + 1}}} \right\rfloor }}}} \right]\\
 &= C\exp \left[ { - {{(1 + \varepsilon )}^2}\frac{{{n_k}\log \log {n_k}}}{{{\left\lfloor {{n_{k + 1}}} \right\rfloor }}}} \right]\\
& \le C\exp \left[ { - {{(1 + \varepsilon )}^2}\frac{{{{(1 + \varepsilon )}^k}\log \log {{(1 + \varepsilon )}^k}}}{{{{(1 + \varepsilon )}^{k + 1}}}}} \right]
\end{aligned}\]`
for infinitely many $k$. From (i), by replacing $X_i$ with $-X_i$ and letting $E =1$, we can get a lower bound on $S_n$, which is
`\[{S_n}>  - 2\sqrt {2n\log \log n} \quad \text{for large enough $n$ a.s.}\]`