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

Travel time is given by Fermat's principle`\[\tau(x,y) = \min\limits_{\Gamma}\int_{\Gamma}\frac{ds}{c(x(s))}. \] `
Derivation of the random travel time model: For $\lambda\ll l\ll L$ seek solution of Helmholtz equation: $u=\alpha e^{iw\tau}$:  

- Travel time $\tau$ solves eikonal equation: $\left|\nabla\tau\right|^2 = \frac{1}{c^2(x)}$.
- Amplitude $\alpha$ solves transport equation $2\nabla\alpha \cdot \nabla\tau +\alpha\Delta \tau =0$.  

The result extends to fairly general fluctuations: stationary, mean zero, ergodic in $z$ (mixing). Diffusion limit theorem: Kohler, Papanicolaou, Varadhan.  

**Scales are important!**  

Cross-range resolution. CINT 

## Synthetic aperture radar imaging - Margaret Cheney
How to get image of the Earth and stars far away  

SAR: developed by engineering community; scattering theory, microlocal, ...  

Antenna on an aircraft sends signals to ground satellites then receives back the reflected signal. Goal: get image on the ground from above (10km $\sim$ small photo)

1951: Carl Wiley, Goodyear  

mid-50: first operational systems  

1960: NASE sponsorship, first digital SAR processors  

78: SEASAT-A: 100 days  

1981: beginning SIR series (shuttle imaging radar)  

SIR-C 1994 Weddell Sea: create false color. Assign different channel to different color: create beautiful picture.  

Satellite: making amazing image of the Earth  
TerraSAR cooper mine in Chile  

Internal waves at Gibraltar. 

ERS-1, ERS-2: 

Airborne systems: AriSAR, LynxSAR: Capitol, Radar projection is not the same as optical projection.  

Outline: standard matheamtical model for radar data (assumes propagation through free space). Image reconstruction from standard model.  

3D Math model: we should use Maxwell's equation, but instead (scalar wave)
`\[\left(\nabla^2-\frac{1}{c^2(x)}\partial_t^2 \right)E(t,x)=i(t,x) \;\text{(source)}\]`
but not good for random medium.  
One thing to need to know: Fundamental solution: Green's solution: outgoing spherical wave (fourier transform of delta function)  

Scattering theory: empty universe, vacuum wave speed. Lippman-Schwinger integral equation. 
`\[E^{sc}(t,x)=\int g(t-\tau,x-z)V(z)\partial_{\tau}^2E(\tau,z)d\tau dz.\] `
Inverse problem: measure scatter field, and $V(z)$. Problem, $V(z)$ is attached to the nearby scatter field.  

Single-scattering and _Born_ approximation: makes inverse problem linear but not good approximation. Math techniques to remove artifacts.

Incident wave: the field from the antenna is $E^{in}$. Real-aperture imaging versus synthetic-aperture imaging. Big antenna: narrow beam (R-A imaging), small antenna: broad beam (S-A imaing): combine data from different location.  

CSU-CHILL: very large antenna disk, plot from different time-delayed data.  


Putting it all together: Fourier Integral Operator (microlocal analysis techniques apply). Similar to seismic inveresion problem.  

Reconstruction a function from its integrals over circles or lines. Brett Borden, Naval. Rdar FIO, Beyklin (JMP '85). Radar application: Nolan & Cheney.   

Random medium is needed

- through foliage (what's in the shadow)
- through sea ice (complicated)
- through ionosphere (complicated, many layers)

CARABAS uses long wavelengths.  

Electromagnetic waves and SEA ICE (salt in water very conductive, like metal).  

Fundamentals of Radar Imaging. 

## Ganesh

Attenuation

## Bal

Stochastic and periodic homogenization
`\[-\nabla\cdot a\nabla u =f;\quad u=g\; \text{on }\partial U\\ -\nabla\cdot a\nabla u+\alpha u =f \]`
We have $a(x)\to a(x/\varepsilon)$. Two-scales: homogenization $\Leftrightarrow$ effective media or macroscopic models.  

We have $a=a\_{\varepsilon}(x)=a(x/\varepsilon)$.   

First setting: $a(y)$ is periodic coefficient, $(y=x/\varepsilon)$.
`\[-\nabla a_{\varepsilon}\nabla u_{\varepsilon}+\alpha u_{\varepsilon}=f \]`
We conjecture $u\_{\varepsilon}[a\_{\varepsilon}]\to\_{\varepsilon \to 0} {\bar u}[{\bar a}]$. Two scales $y=x/\varepsilon$ (fast scale). Two scale expansion $u\_{\varepsilon}(x)=u(x,y)$$\;=u(x,x/\varepsilon)$. This is an ansatz, maybe wrong but good guess. Then write equation for $u(x,y)$, then get equations for different scales. 

Fredholm alternative: spectral gap; 0 is the first one.  

Effective constant
`\[a^* = \left({\mathbb E}\frac{1}{a} \right)^{-1} \]`
$a(y)$ must be elliptic between $\lambda$ and $\Lambda$. We have a result basically saying sharpness
`\[ \lambda \le \mathbb E(a^{-1})^{-1} \le a^*\le \mathbb E a\le \Lambda\] `
