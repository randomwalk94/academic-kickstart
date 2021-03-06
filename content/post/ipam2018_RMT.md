+++
title = "Random Matrices in Los Angeles"

date = 2018-05-14
draft = false

tags = ["research", "conference", "summer 2018", "random matrix theory", "free probability"]
summary = "Notes on some of the topics presented at the Workshop: Random Matrices and Free Probability Theory at IPAM during summer of 2018."

[header]
image = "/ipam2018.jpg"
caption = "Image credit: [**HDwallsource**](https://hdwallsource.com/awesome-los-angeles-wallpaper-41390.html/awesome-los-angeles-wallpaper-41390)"

+++

Website for the workshop: [Workshop III: Random Matrices and Free Probability Theory](http://www.ipam.ucla.edu/programs/workshops/workshop-iii-random-matrices-and-free-probability-theory/).

I will not (and cannot) cover everything that was presented at the conference. Here are some of the materials that I found useful and interesting.

## Table of contents
<!-- TOC -->

- [Table of contents](#table-of-contents)
- [Brown measure](#brown-measure)
- [Wigner-Dyson-Mehta conjecture](#wigner-dyson-mehta-conjecture)
- [Quantum Unique Ergodicity conjecture](#quantum-unique-ergodicity-conjecture)
- [Brownian motions on Lie groups](#brownian-motions-on-lie-groups)
- [Chinese restaurant process](#chinese-restaurant-process)
- [CUE field](#cue-field)
- [Laplace deviation principle/Free entropy](#laplace-deviation-principlefree-entropy)
- [Dan-Virgil Voiculescu](#dan-virgil-voiculescu)
- [Compressed sensing/Sparsity](#compressed-sensingsparsity)
- [Ofer Zeitounni](#ofer-zeitounni)
- [Random matrices with prescribed eigenvalues](#random-matrices-with-prescribed-eigenvalues)

<!-- /TOC -->

## Brown measure

One first needs the framework of [free probability theory](https://en.wikipedia.org/wiki/Free_probability). I have written down some notes about this subject in a [blog post](/post/free_probability).

## Wigner-Dyson-Mehta conjecture

## Quantum Unique Ergodicity conjecture

## Brownian motions on Lie groups

A **Brownian motion** $(U\_t)\_{t\ge 0}$ on the unitary group $\mathbb U\_N$ is a Markov process starting at $I\_N$ whose **generator is the Laplacian** $\frac{1}{2}\delta\_{\mathbb U\_N}$ for a certain metric.

For other Lie groups: Levy (2011), Cébron, Kemp (2013), Ulrich (2015). For more general situations: Cébron (2016), Gabriel (2015). The set of trace polynomials has to be replaced by the set of traffic operations (in the sense of Camille Male).

The Segal-Bargmann transformation (1958). $q$-Gaussian law (Bozejko-Speicher, 1991). $q$-deformation.

## Chinese restaurant process

## CUE field
Arguin-Belius-Bourgade-Soundararajan-Radziwill'16 on the Riemann $\zeta$ function.

## Laplace deviation principle/Free entropy
Yoann Dabrowski

## Dan-Virgil Voiculescu
Ben Arous-V. Free Max-stable Laws. Pareto-distribution.

## Compressed sensing/Sparsity
Candes, Romberg, Tao '06, Donoho. Restricted isometry property. Khintchine inequality.

## Ofer Zeitounni
Small pertubations of Toeplitz random matrices. Trefethen - pseudo-spectrum. Spectrum stability for symmetric matrices. No controls on non-Hermitian matrices. Ginibre complex  matrices. Sniady's theorem ('02). In particular, some sequence of noise regularizes empirical measure to Brown measure.

## Random matrices with prescribed eigenvalues
Set of eigenvalues $\Lambda=\\{\lambda_1,\lambda_2,\ldots,\lambda_n \\}$. Let $M^{\Lambda}_n(\mathbb R)= \text{ symmetric matrices over } \mathbb R \text{ with eigenvalues in }\Lambda$. Random matrix $M=UI\_{\Lambda}U^*$ where $I\_{\Lambda}$ is diagonal matrix with the prescribed eigenvalues and $U$ is random unitary matrix with respect to Haar measure.

Schur-Horn theorem: If $(d\_i)$ and $\lambda\_i$ are diagonal entries and eigenvalues of complex Hermitian matrices, then $(d\_i)\prec (\lambda\_i)$. The converse statement is true.