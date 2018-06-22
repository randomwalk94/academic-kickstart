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

## Friday-June 15-2018
1\. Progressively measurable stochastic process (vs adapted process) (look into [link](http://page.math.tu-berlin.de/~scheutzow/WT3main.pdf))  

2\. Martin Hairer's regularity structures ([Link](http://www.hairer.org/papers/mSHE.pdf)): Decomposition of heat kernel (Lemma 5.5, Theorem 5.12). "Canonical model" (Proposition 8.27). Renormalization is to "correct" Picard iteration at each step. To see how renormalization works, consider the term `$({\mathcal D}{\mathcal I}(\Xi))^2$`: $\Xi$ is the white noise, thought of as derivative of Brownian motion; hence, the action ${\mathcal D}{\mathcal I}$ on $\Xi$ basically recovers Brownian motion. To correct this, we have
`\[M(({\mathcal D}{\mathcal I}(\Xi))^2)=({\mathcal D}{\mathcal I}(\Xi))^2-\frac{c}{\varepsilon} \]`
where $M=I-cL-\cdots$ where $L$ represents the action of "removing" Brownian motion.  

3\. **Problem about feeble fish**. In homogenization theory, the underlying vector field is set to be random. Roughly speaking, consider a (random) vector field $V:(\text{space},\text{time})\to \mathbb R$. Consider the following dynamics:
`\[dX=Vdt,\quad \text{(or in discrete settings)}\quad X_{n+1}=X_n+V(X_n,n).\]`
We would expect in the long time, $X\sim \mathbb E(V) \cdot t$, or equivalently, $\frac{X}{t}\to \mathbb E(V)$ where the expectation is respect to the underlying probability measure. The main question is under what condition this would hold true.  

> Always to think about the purpose of defining an object.  

We first work in the discrete settings. To even talk about expectation $\mathbb E$, we must have _stationarity_ in both space and time. That's the first condition. We will consider its "ergodicity" (the relationship between time and space average). Let $W:\mathbb Z^2\to \mathbb Z^2$ is a *deterministic* velocity (with compact support to ensure convergence later), and $\xi\_{ij}$ be i.i.d random variables (taking only $0$, $1$ or any finite set of values). One way to construct the random velocity $V$ is as follows
`\[V(x,t)=\sum\limits_{ij}\xi_{ij}V(x+i,t+j).\]`
Consider the (canonical) space-time shift $T\_{ij}:\mathbb Z^2\to \mathbb Z^2$ 
`\[T_{ij}(x,t)=(x+i,t+j).\]`
These shifts are measure-preserving `$V(x,t,T_{ij}\omega)=V(x+i,t+j,\omega).$` The claim is that $V$ is strongly mixing with respect to these shifts. And we indeed get that $X\_n/n\to \mathbb E(V)$ ([link](https://arxiv.org/abs/1712.08395)). The main question is can we reduce the strong mixing condition to just being ergodic, or is there a counterexample? "Ergodic" means that 
`\[\frac{1}{N}\sum\limits_{n=1}^{N} V(T_{ij}^{n}(x,t)) \to \int Vd\mathbb P\]`
where $\mathbb P$ is the underlying probability measure. Do we have
`\[\frac{1}{N}\sum\limits_{n=1}^{N} V(X_n,n)\to\int Vd\mathbb P\;\;\]`
as $X\_n$ follows the dynamics $X\_{n+1}=X\_n $$\;+ \;V(X\_n,n)$? This is a type of questions in Random Walks in Random Environment.

4\. How to solve stochastic heat equation: [link](https://arxiv.org/pdf/1402.2618.pdf)  

5\. [Regularity structures and renormalisation of FitzHugh–Nagumo SPDEs in three space dimensions](https://arxiv.org/abs/1504.02953)

## Sunday-June 17-2018
1\. The Birkhoff-von Neumann theorem states that the set of $n \times n$ doubly stochastic matrices (non-negative matrices whose every row and every column sums to $1$) is convex, and that the extremal points of the set are (all) the permutation matrices.  

2\. The Hoffman-Wielandt inequality states that for any two $n \times n$ normal matrices $A$, $B$, with sets of eigenvalues $\lambda_1(X),\; \lambda_2 (X),\;\ldots,\; \lambda_n(X)$ for `$X \in \{A, B\}$`, there exists a permutation $\sigma \in S\_n$ such that `\[ \sum_{i=1}^n |\lambda_i(A) - \lambda_{\sigma(i)}(B)|^2 \leq \text{Tr}\left((A-B)(A-B)^*\right). \]` 
_Proof._ (kind of) Express `$\text{Tr}\left((A-B)(A-B)^*\right)$` as a function on doubly stochastic matrices. Then use Birkhoff-von Neumann theorem to achieve the minimum and maximum.

## Thursday-June 21-2018
1\. Bipartite biregular model $(m,n,d\_1,d\_2)$, $md\_1=nd\_2$. Eigenvalues of the adjency matrix $A$ are $n-m$ zeros and $\pm \sigma_i$ (singular values of $X$). Models for $X^TX$: Wishart.  

2\. Extremal eigenvalues of graphs. Graphs matrices:  

- adjacency matrix $A\_{ij}=\lambda\_{ij}$
- Laplacian matrix $L=I-D^{-1}A$ where $D=\text{diag}(\deg(v_i))$, note that a graph defines a Markov chain: $D^{-1}A$ is Markov matrix for graph.  

3\. Cauchy-Binet formula: Let $A$ be an $m\times n$ matrix and $B$ be an $n\times m$ matrix. Let $1\le j\_1,i\_2,\ldots,j\_m\le n$. Let $A\_{j\_1i\_2\ldots j\_m}$ denote the $m\times m$ matrix consisting of columns $j\_1,i\_2,\ldots,j\_m$ of $A$. Let $B\_{j\_1i\_2\ldots j\_m}$ denote the $m\times m$ matrix consisting of rows $j\_1,i\_2,\ldots,j\_m$ of $B$. Then
`\[\det(AB)=\sum\limits_{1\le j_1<j_2<\ldots<j_m\le n}\det(A_{j_1j_2\ldots j_m})\det(B_{j_1j_2\ldots j_m}) \]`
Using this we can prove the Jacobi-Trudi identity. Let $h\_m(x)=h\_m(x\_1,x\_2,\ldots)$ denote the complete homogeneous symmetric polynomial. The Jacobi-Trudi states that
`\[s_{\lambda}=\det(h_{\lambda_i-i+j})_{i,j=1}^{l(\lambda)} \]`
where `$s_{\lambda}(x_1,\ldots,x_n)$` is Schur polynomial defined as 
`\[s_{\lambda}(x_1,\ldots,x_n) = \frac{\det(x_i^{\lambda_j+n-j})}{\prod\limits_{i<j}(x_i-x_j)}\] `
The proof proceeds in three steps  

- Prove that if `$f(u)=\sum\limits_{m=0}^{\infty} f_mu^m$`, then using Cauchy-Binet,
`\[f(x_1)f(x_2)\ldots f(x_n) =\sum\limits_{\lambda:l(\lambda)\le n} \det(f_{\lambda_i-i+j})_{i,j=1}^{l(\lambda)}s_{\lambda}(x_1,\ldots,x_n). \]`
- Let $f\_m=h\_m(y_1,\ldots,y_n)$ to show that 
`\[\prod\limits_{i,j}\frac{1}{1-x_iy_j} = \sum\limits_{\lambda}\det(h_{\lambda_i-i+j}(y_1,\ldots,y_n))_{i,j=1}^{l(\lambda)}s_{\lambda}(x_1,\ldots,x_n) .\]`
- Finish by using the Cauchy identity
`\[\sum\limits_{\lambda}s_{\lambda}(x)s_{\lambda}(y)=\prod\limits_{i,j}\frac{1}{1-x_iy_j}. \]`
Reference: [Symmetric Functions and Hall Polynomials](https://pdfs.semanticscholar.org/0613/1de77b4268cc9d4334a661846c42873cb8e4.pdf) by MacDonald.  

4\. The $\lambda\_k$ eigenvalue tells how a graph can be separated into $k$ connected components.

## Friday-June 22-2018
1\. Ihara-Bass formula: For non-backtracking matrix $B$ and adjacency matrix $A$ of a graph $(G,E,V)$, we have for every $z\in \mathbb C$
`\[\det(B-zI)=(1-z^2)^{|E|-|D|}\det(z^2I-zA+D)\]`
where $D=\text{diag}(\det(v\_i)-1)$.