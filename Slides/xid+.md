XID+: The probabilistic de-blender for confusion dominated maps, Hurley et al 2017
* Uses Bayesian Inference to get FULL posterior
* Provide a natural framework to introduce additional prior information
* Allows more accurate estimate of flux density errors for each source
* Provides a platform for doing science with the maps rather than catalogues


## 1. Model building
Build a probabilistic model of our data

note:
Generative model: our model is capable of generating the replicated data


<!-- .slide: data-transition="slide in fade out" -->
![](Slides/assets/prob_graph_mod1.png?raw=true)


<!-- .slide: data-transition="fade in fade out" -->
![](Slides/assets/prob_graph_mod2.png?raw=true)


<!-- .slide: data-transition="fade in fade out" -->
![](Slides/assets/prob_graph_mod3.png?raw=true)


## 2. Inference
Uses Probabilistic Programming language, Stan
![](http://mc-stan.org/images/stan_logo.png?raw=true)

note:
Allows complex probabilistic models to be built, without worrying about how to do inference. Includes HMC, a MCMC routine that uses gradient information to efficiently sample parameter space.


<!-- .slide: data-transition="slide in fade out" -->
<iframe data-autoplay width="2600" height="400" src="Slides/assets/prior_animation_key.m4v"></iframe>

note:
Our model is generative, i.e. we can generate the expected data given certian values of parameters
* Each frame is a sample from the prior.. 
* it is one of the possible maps we might expect to observe, given our prior information
* Movie shows the variation in possible maps we could observe, given our prior


<!-- .slide: data-transition="fade in fade out" -->
<iframe data-autoplay width="2600" height="400" src="Slides/assets/post_animation_key.m4v"></iframe>

note:
Once we infer our model
Parameters now have posterior probability function (i.e. update from prior, given data)
* Each frame is a sample from the posterior.. 
* it is one of the possible maps we might expect if we were to re-observe
* Movie shows the variation in possible maps we could re-observe


<!-- .slide: data-transition="fade in fade out" -->
![](Slides/assets/real_map.png?raw=true)<!-- .element height="78%" width="78%"-->


![](Slides/assets/XID+_vs_DESPHOT_joint.png?raw=true)<!-- .element height="65%" width="65%"-->


## 3. Model Checking
### Posterior Predictive Checking
$P(D^{rep}|M,D)=\int P(D^{rep}|M,\theta)P(\theta|M,D)d\theta$<!-- .element: class="fragment" data-fragment-index="1" -->
$p_B=P(T(D^{rep},\theta)\geq T(D,\theta)|M,D)$<!-- .element: class="fragment" data-fragment-index="2" -->

note:
* How do most people do model checking.. plot best fit, use max likelihood to get residual?
* We have full uncertianty information on parameters and how that feeds down to data..
* we can replicate data and create distribution rather than one value e.g. movie
* idea of PPCs is to come up with a test you can apply to data to test model.. graphical
* create p value: measures prob. model returns values > than data


### XID+Bayesian P-value maps
![](Slides/assets/post_pred_pix.png?raw=true)


XID+Bayesian P-value and standard MLM residual maps
![](Slides/assets/res_comp.png?raw=true)


Maps reveal 'Hidden' FIR sources
![](Slides/assets/bayes_scuba2.png?raw=true)<!-- .element height="80%" width="80%"-->

note:
Herschel maps have already revealed numerous high redshift dusty starburst galaxies, including  one at highest redshift, z=6.34. However, these have been the most obvious, brightest examples..

Bayesian P-value maps strip away contribution from galaxies we already know about, to reveal other FIR sources. Already shown that many of these pvalue sources are real and can be seen by SCUBA2


The multiplicity of 250-$\mathrm{\mu m}$ $\mathit{Herschel}$ sources in the COSMOS field, Scudder et al. 2016

![](Slides/assets/multiplicity.png?raw=true)<!-- .element height="70%" width="70%"-->

note:
360 250 sources above 30 mJy,1 24 counterpart and >=1 3.6 counterpart

low 250 source fluxes (30−45 mJy),brightest components assigned larger fraction of total 250 flux

Above 45 mJy brightest components contain 45 per cent of the total 250 source flux.

If both 1st and 2nd brightest components considered, < 45 mJy, 90% of the 250 source flux is accounted for

At larger fluxes, 2 brightest components contain only 70% of total flux
