+++
title = "Research Diary July2018"

date = 2018-07-01
draft = false

tags = ["research", "diary", "summer 2018"]
summary = "Daily notes for research."

[header]
image = ""
caption = ""

+++

## Tuesday-July 24-2018
1\. (Sloppy formulation) There are two KPZ universality conjectures  

1. (_Weak KPZ universality conjecture_) For any tunable asymetric model (e.g ASEP with $\text{down}\to\text{up}$ probability $p$ and $\text{up}\to\text{down}$ probability $q$), let the asymmetry $\alpha=p-q=\varepsilon^{1/2}\to 0$ and perform $1:2:4$ scaling, the model will converge to KPZ equation.
2. (_Strong KPZ universality conjecture_) For a large class of growth models, performing $1:2:3$ scaling `$h^{\varepsilon}:=\varepsilon^{1/2}h(\varepsilon^{-3/2}t,\varepsilon^{-1}x)$` will converge to the _KPZ fixed point_ (which is a $1:2:3$ invariant Markov process). 

Performing $1:2:4$ scaling converges to Edward-Wilkinson fixed point. Connecting the KPZ fixed point and E-W fixed point in the "space of Markox processes" is the unique curve, KPZ equation.  

The weak conjecture is "techincally solved" by using regularity structures (or by Gubinelli's paracontrolled method) since we now know what it means to be a solution to KPZ and what is close to be a solution. What remains to be proved will be done in the next five years.  

2\. KPZ equation
`\[\partial_th = \alpha(\partial_x h)^2 + \partial_x^2h+\xi. \] `
For general non-linear growth term $F(\partial_xh)$ (this makes sense as this does not depend on time and only cares about what surface it is standing on), using Taylor expansion, we get that
`\[F(t)=F(0) + tF'(0)+\frac{t^2}{2}F''(0)+\ldots. \]`
The first two terms can be ignored by affine transformation. Hence, the most significant term is of second-order.  

3\. If $F$ has two equal and stable wells ($\alpha=0$), we will get Edwards-Wilkerson equation (commonly known as OU process or _additive stochastic heat equation_, but should not be called like that). 
` \[ \partial_th = \partial_x^2h +\xi\]`
which makes sense in every dimension (but only in $1+1$ dimension, the solution is function-valued). Solution is of the form $\text{Brownian motion }+px$; hence, it is $1/2$-space and $1/4$-time (proven by Kolmogorov criteria, two-point regularity induces regularity on the process). This equation is $1:2:4$ scaling invariant.  

Performing $1:2:4$ scaling, `$h^{\varepsilon}=\varepsilon^{1/2}h(\varepsilon^{-2}t,\varepsilon^{-1}x)$`, on KPZ gives 
`\[\partial_t h^{\varepsilon} = \frac{1}{\varepsilon^{1/2}}(\partial_xh^{\varepsilon})^{2}+\partial_x^2h^{\varepsilon}+\xi. \]`
Hence, KPZ is not $1:2:4$ invariant. However, it is believed that (two-sided) Brownian motion is still invariant under KPZ (but no proof) (reference: [Funaki-Quastel](https://arxiv.org/pdf/1407.7310.pdf).) 

Performing dynamic scaling `$h^{\varepsilon}=\varepsilon^{1/2}h(\varepsilon^{-z}t,\varepsilon^{-1}x)$`, we obtain
`\[\partial_t h^{\varepsilon} = \varepsilon^{3/2-z}(\partial_xh^{\varepsilon})^{2}+\varepsilon^{2-z}\partial_x^2h^{\varepsilon}+\varepsilon^{(2-z)/2}\xi.\]`
Hence, setting $z=3/2$ gives non-trivial limit.  

4\. Fluid dynamics viscosity plays a role of statistical mechanics temperature.  

5\. History of Burgers equation with random forcing: Sinai, early 90's, $\chi>0$; Khanin, Mazel, sinal, $\chi=0$ (on the circle $\mathbb T^1$) with continuous time
`\[F_{\omega}(t,x)=\sum\limits_{k=1}^nF_k(x)\xi_k(t) \]`
where $\xi\_k$'s are white noise. In the paper, established One Force One Solution (1F1S) principle on each ergodic component (sloppy: "ergodicity" means forgetting the initial data). [EKMS2000] 1F1S on $I\_c$, for all $c\notin \mathbb R$.  

6\. Hyperbolicity. Busemenn function.  

7\. (Subadditive ET) If $\theta$ is an ergodic transformation of $\Omega,\mathcal{F},\mathbb P$ and $(X\_n)\_{n\in \mathbb N}$ are $L^1$ random variables such that $X\_{n+m}(\omega)\le X\_n(omega)+X\_m(\theta^n\omega)$. Let $\alpha=\inf \mathbb E X\_n/n$, then almost surely $X\_n/n\to \alpha$.