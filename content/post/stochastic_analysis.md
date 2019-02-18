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

Stochastic calculus is the theory of _stochastic processes_. Just like classical calculus being the study of functions, stochastic calculus provides mechanism to operate on stochastic processes, which are in essence _random functions_.

The book that I enjoyed reading the most is the one by [Fabrice Baudoin](https://sites.google.com/site/fabricebaudoinwebpage/books), "Diffusion processes and Stochastic calculus." It has neat presentation, natural motivation built leading to each topic which makes technical stuff less "technical," and good comments as well as references at the end of each chapter. Another well-written and detailed lecture notes are due to [Andreas Eberle](https://wt.iam.uni-bonn.de/fileadmin/WT/Inhalt/people/Andreas_Eberle/StoAn15/StochasticAnalysis2015.pdf). You can also find more at [Davar Khoshnevisan's website](http://www.math.utah.edu/~davar/lecture-notes.html).

In this post I'm just going to review materials that I once found challenging or confusing. Therefore, anything below is subject to my personal experience. A more compresenhive treament of course can be found in any book on stochastic processes, or in the one I just recommended. A list of available references is too long for me to include here, and I don't want to impose biases on books that I haven't read thoroughly.

To keep things at the intuitive level and less involved (which I prefer when learning this subject), I will not try to write all the details and only do so when they are really needed. 

## What are stochastic processes?  
In real analysis, one starts diving into the "epsilon"-world by studying _sequences_. Then we define what it means to have a sequence converge and so on. A sequence (of any objects) can be thought of as a function of _discrete_ time. More precisely, the sequence $(x\_n)\_{n=1}^{\infty}$ (let's say, of real numbers) is nothing but a function $f:\mathbb N\to \mathbb R$ defined as $f(i)=x\_i$ for $i\ge 1$. Then a natural extension is to have a function of _continuous_ time; that's why we have a general function defined as $f:\mathbb R\to \mathbb R$. 

To transfer the analogy to the stochastic world, we replace the destination set $\mathbb R$ by the set of random variables (which are already well-defined in some probability space). Hence, stochastic processes are just _sequences of random variables_, and are either _discrete_ or _continuous_ time. When time is continuous, stochastic processes are sometimes called _random functions_. Each realization or instance of a random function is called a _path_. Just to quote [Joseph Doob](https://en.wikipedia.org/wiki/Joseph_L._Doob) (an American probabilist who is most famous for his work on [martingales](https://en.wikipedia.org/wiki/Martingale_(probability_theory))),  

>A stochastic process is any process running along in time and controlled by probability laws... more precisely any family of random variables where a random variable... is simply a measurable function...

I believe before going to the whole theory, this is the way we should think about the objects that we will study. Then everything will come more naturally. 

## The Kolmogorov continuity theorem  

## Martingales and Doob's theorems

## Brownian motions

### Law of iterated logarithms

### Donsker theorem

### White noise
The term ‘white noise’ arises from the spectral theory of stationary random processes, according to which white noise has a ‘flat’ power spectrum that is uniformly distributed over all frequencies (like white light). This can be observed from the Fourier representation of Brownian motion, where a formal term-by-term differentiation yields a Fourier series all of whose coefficients are Gaussian random variables with same variance.  

White noise is a sound with equal intensity at all frequencies within a broad band. Rock music, the roar of a jet engine, and the noise at a stock market are examples of white noise. We use the word white'' to describe this kind of noise because of its similarity to white light'' which is made up of all different colors (frequencies) of light combined together. In applied science white noise is often taken as a mathematical idealization of phenomena involving sudden and extremely large fluctuations.
## Markov processes
### Semigroup

### Ornstein–Uhlenbeck process

The O-U process as a model for volatility: [notes](http://stat.math.uregina.ca/~kozdron/Teaching/Regina/441Fall14/Notes/L31-32-Nov19.pdf).

## Ito calculus

### The characteristic function for a diffusion

How to obtain the the characteristic function for a diffusion without solving the SDE: [notes](http://stat.math.uregina.ca/~kozdron/Teaching/Regina/441Fall14/Notes/L33-34-Nov24.pdf).
### Burkholder–Davis–Gundy inequalities

### Girsanov theorem

## SDE