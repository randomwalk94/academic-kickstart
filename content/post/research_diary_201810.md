+++
title = "Research Diary October2018"

date = 2018-10-01
draft = false

tags = ["research", "diary", "fall 2018"]
summary = "Daily notes for research."

[header]
image = ""
caption = ""

+++

## Sunday-October 3-2018  
1\. Reeb graph, Hamiltonian. It was shown that the non-Markovian processes $\Gamma(X_t^{x,\varepsilon})$ converge in distribution, as $\varepsilon\to 0$ to a disffusion on the graph. Reeb:
`\[\Gamma: \mathcal{T}\to G, \quad \Gamma(x)=(i,|H(x)|)\;\text{if }x\in \bar U_i. \]`

2\. (Pertubed test function) To prove tightness of a sequence of processes $\{x^{\varepsilon}(\cdot)\}$, we define an operator ${\hat A}{}^{\varepsilon}$ on $x^{\varepsilon}$ which has properties similar to those of an infinitesimal operator of a Markov process. If $A$ is the operator for the limit process $x(\cdot)$, we can then compare ${\hat A}{}^{\varepsilon}f^{\varepsilon}(\cdot)$ with $Af(x^{\varepsilon}(\cdot))$, where $f^{\varepsilon}(\cdot)$ is an appropriate small perturbation of $f(\cdot)$. Under some suitable conditions, if ${\hat A}{}^{\varepsilon}f^{\varepsilon}(\cdot)-Af(x^{\varepsilon}(\cdot))\to 0$ for all smooth $f$ as $\varepsilon\to 0$, then $x^{\varepsilon}(\cdot)$ will converge (weakly) to $x(\cdot)$.

## Wednesday-October 10-2018  
1\. Two ways to treat these processes:

- Solutions to SDE.
- Solutions to _martingale problem_.

It is often easier to show that a process that is the limit of s sequence of processes satisfies a martingale problem than it is to show that it satisfies an SDE.

2\. The process $\langle x\rangle$ is the _quadratic variation_ of $x(\cdot)$ if it is the _unique continuous nondecreasing process_ adapted to $\mathcal{F}\_t$ and that $x^2(\cdot)-\langle x\rangle$ is an $\mathcal{F}\_t$-martingale. Precisely,
`\[\sum[x(t^n_{i+1})-x(t^n_i)]^2 \to \langle x\rangle(t)\;\;\text{in probability.} \]`
For two processes $x\_1(\cdot)$ and $x\_2(\cdot)$, $\langle x_1,x_2\rangle(t)$ is called the _quadratic covariation_ such that 
`\[x_1(\cdot)x_2(\cdot)-\langle x_1,x_2\rangle (\cdot)\;\;\text{is a martingale.} \]`