+++
title = "Research Diary June2018"

date = 2018-06-01
draft = false

tags = ["research", "diary", "summer 2018"]
summary = "Daily notes for research."

[header]
image = ""
caption = ""

+++

## Thursday-June 14-2018
1\. A survey on KPZ and universality class by Ivan Corwin: [arXiv 1106.1596](https://arxiv.org/pdf/1106.1596.pdf). Another notes by Ivan Corwin: [Exact solvability of some SPDEs](https://www.math.columbia.edu/~corwin/MSRIJuly2014.pdf).
The stochastic heat equation (SHE) with multiplicative noise looks like (in differential form; formally, no exact meaning at the beginning)  
`\[\left\{ \begin{array}{l} {\partial _t}z = \frac{1}{2}{\partial _{xx}}z + z\xi \\ z(0,x) = {z_0}(x) \end{array} \right.\]`
where $z:\mathbb R\_{+}\times \mathbb R \to \mathbb R$ and $z_0$ is (possibly random) initial data which is independent of the white noise $\xi$ (will be described in detail later). The only thing to keep in mind right now is $\xi$ can be thought of as a random distribution. (SHE) makes sense by the following notion of solution.  
&nbsp;   
**Definition.** *A mild solution to the SHE for all $t>0$ and $x\in \mathbb R$ is $z(\cdot,\cdot)\in L^2(\Omega,\mathcal{F},\mathbb P)$ satisfies the Duhamel formulation*  
`\[z(t,x)=\int_{\mathbb R}p(t,x-y)z_0(y)dy+\int_0^t\int_{\mathbb R}p(t-s,x-y)z(s,y)\xi(s,y)dyds \] `
*where $p(t,x)=\frac{1}{\sqrt{2\pi t}}e^{-x^2/2t}$ is the heat kernel or fundamental solution to $\partial\_tp=\partial\_{xx}p$ with $p(0,x)=\delta\_{x=0}$. Also, we must have a priori that `$\int_0^t\int_{\mathbb R}p^2(t-s,x-y){\mathbb E}[z^2(s,y)]dyds<\infty$` for the Ito integrals (stochastic integrals) to make sense and finite.*  

2\. sd sd  

3\. s sd
