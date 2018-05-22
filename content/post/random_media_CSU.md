+++
title = "Random Media at Colorado"

date = 2018-05-18
draft = false

tags = ["research", "conference", "summer 2018", "stochastic partial differential equations", "probability theory", "inverse problem"]
summary = "Notes for the summer school on Random Media at Colorado State Univeristy."

[header]
image = "/random_media.jpg"
caption = "Image credit: [**map028**](http://www.map028.com/single/190739287-paint-amp-amp-wallpapers.html)"

+++

Website for the summer school: [Summer School Waves and Particles in Random Media: Theory and Applications](http://www.math.colostate.edu/~pinaud/SummerSchool/school.html).

The summer school was held on campus of Colorado State University in Fort Collins.

## Borcea  

Weak scattering regime in open environments. Stronger regimes require an in depth study of waves in random media.  

Coherent imaging: Transport mean free part-quantify the decay of the mean.  

CINT passive arrays. Model of random medium:
`\[\frac{1}{c^2(x)} = \frac{1}{c_0^2} \left[1+\sigma \mu\left(\frac{x}{l} \right) \right] \] ` 
$\mu(x)$ is mean zero, statistically homogeneous. Model applied to clear air turbulence and captures only _wave front distortions._ The model is assumed in the adaptive optics methodology.  

Travel time is given by Fermat's principle
`\[\tau(x,y) = \min\limits_{\Gamma}\int_{\Gamma}\frac{ds}{c(x(s))}. \] `
Derivation of the random travel time model: For $\lambda\ll l\ll L$ seek solution of Helmholtz equation: $u=\alpha e^{iw\tau}$:  

- Travel time $\tau$ solves eikonal equation: $\left|\nabla\tau\right|^2 = \frac{1}{c^2(x)}$.
- Amplitude $\alpha$ solves transport equation $2\nabla\alpha \cdot \nabla\tau +\alpha\Delta \tau =0$.  

The result extends to fairly general fluctuations: stationary, mean zero, ergodic in $z$ (mixing). Diffusion limit theorem: Kohler, Papanicolaou, Varadhan.  

**Scales are important!**  

Cross-range resolution