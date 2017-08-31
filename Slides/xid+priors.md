## 4. Model Understanding and improvement

* More galaxies we fit, better model
* Adding more galaxies increases degeneracy on flux
### Solution:
Add more prior information

note:
* We have more situations when sources are close
* We have a similar situation as my example of one data point
* Different ways of adding prior


<!-- .slide: data-transition="slide in fade out" -->
![](Slides/assets/XID+250_350_500_joint.png?raw=true)<!-- .element height="60%" width="60%"-->


<!-- .slide: data-transition="fade in slide out" -->
![](Slides/assets/XID+250_350_500_joint_2.png?raw=true)<!-- .element height="60%" width="60%"-->


## What should we add as prior?
* Fit ancillary data with SEDs, get more informative prior for SPIRE (i.e. normal distribution rather than uniform)
* Introduce SED models into XID+
* Add empirical relationship model into XID+ (i.e. fluxes constrained to multi-D Gaussian)


De-blending Deep $\mathit{Herschel}$ Surveys: A Multi-wavelength Approach, Pearson et al. 2017.
* Marginalised flux priors for SPIRE bands<!-- .element: class="fragment" data-fragment-index="1" -->
* Use Cigale to fit optical and NIR ancillary data<!-- .element: class="fragment" data-fragment-index="2" -->


![](Slides/assets/pearson.png?raw=true)


<!-- .slide: data-transition="slide in fade out" -->
XID+CIGALE

![](Slides/assets/prob_graph_mod4.png?raw=true)

note:
No covariance information between bands


<!-- .slide: data-transition="fade in slide out" -->
XID+SEDs

![](Slides/assets/prob_graph_mod5.png?raw=true)


![](Slides/assets/Joint_SPM.png?raw=true)<!-- .element height="60%" width="60%"-->


XID+Empirical prior

Learn empirical prior from the data..
![](Slides/assets/empirical.png?raw=true)


### Priors are powerful..

* With power, comes great responsibility!
* Any prior used to make catalogue should be consistent with any step after

note:
Any prior I have used in carrying out source extraction, must be consistent with any analysis later.
e.g. SED fitting models must be consistent with my SED prior
* ideal solution. science with maps
