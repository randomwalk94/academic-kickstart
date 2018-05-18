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
Since  ${X_i} \sim N(0,1)$. We note that the above holds if it holds for a subsequence $n_k$,
`\[\begin{aligned}
{\bf{P}}[{S_{{\left\lfloor {{n_{k + 1}}} \right\rfloor }}} > (1 + \varepsilon ){L_{{n_k}}}]& = {\bf{P}}\left[ {\frac{{{S_{{\left\lfloor {{n_{k + 1}}} \right\rfloor }}}}}{{\sqrt {{\left\lfloor {{n_{k + 1}}} \right\rfloor }} }} > (1 + \varepsilon )\frac{{\sqrt {2{n_k}\log \log {n_k}} }}{{\sqrt {{\left\lfloor {{n_{k + 1}}} \right\rfloor }} }}} \right] \\&\le C\exp \left[ { - \frac{1}{2}{{(1 + \varepsilon )}^2}\frac{{2{n_k}\log \log {n_k}}}{{{\left\lfloor {{n_{k + 1}}} \right\rfloor }}}} \right]\hspace{3em} (*)\\
 &= C\exp \left[ { - {{(1 + \varepsilon )}^2}\frac{{{n_k}\log \log {n_k}}}{{{\left\lfloor {{n_{k + 1}}} \right\rfloor }}}} \right]\\
& \le C\exp \left[ { - {{(1 + \varepsilon )}^2}\frac{{{{(1 + \varepsilon )}^k}\log \log {{(1 + \varepsilon )}^k}}}{{{{(1 + \varepsilon )}^{k + 1}}}}} \right]\\
 &= C(\log (1+\E))^{-(1+\E)}{k^{ - (1 + \varepsilon )}}=C_1{k^{ - (1 + \varepsilon )}}.
\end{aligned}\]`