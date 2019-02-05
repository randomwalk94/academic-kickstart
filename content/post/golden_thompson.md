+++
title = "Notes on Golden-Thompson trace inequality"

date = 2019-02-05
draft = false

tags = ["linear algebra", "statistical physics"]
summary = "Some notes for arguably the most powerful trace inequality $\\text{tr}\\exp(A+B)\\le \\text{tr} \\exp(A)\\exp(B)$."

[header]
image = ""
caption = ""

+++

The Golden-Thompson trace inequality states that for any two Hermitian matrices $A$ and $B$ we have
`\[ \text{tr}\exp(A+B)\le \text{tr} \exp(A)\exp(B).\]`
Equality holds when $A$ and $B$ commutte; in fact, this is the only case equality occurs.  

I first read about this inequality via a blog post by [Lior Pachter](https://liorpachter.wordpress.com/2018/10/05/rate-changes-decrease-substitutions/) of Caltech. He interpreted the inequality in the context of substitution matrices used in analyzing DNA mutations on a [phylogenetic tree](https://www.khanacademy.org/science/high-school-biology/hs-evolution/hs-phylogeny/a/phylogenetic-trees).

A thorough discussion can be found on [Terence Tao's blog](https://terrytao.wordpress.com/2010/07/15/the-golden-thompson-inequality/).  

The inequality is itself interesting in the mathematical standpoint as it gives a qualitative comparision between two related expressions $\exp(A+B)$ and $\exp(A)\exp(B)$. One can ask for generalizations to three or higher number of matrices. [Elliott H. Lieb](https://en.wikipedia.org/wiki/Elliott_H._Lieb) found a three-matrix-version of the inequality in his paper [_Convex trace functions and the Wigner-Yanase-Dyson conjecture_](https://www.sciencedirect.com/science/article/pii/000187087390011X) (The generalization is at the bottom of page 282.). I refer to the paper of [Sutter, Berta, and Tomamichel](https://arxiv.org/abs/1604.03023) and references therein for further discussion.
