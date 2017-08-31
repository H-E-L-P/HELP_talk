### Legacy requires multi-$\lambda$ approach

note:
Perhaps more than any other wavelength regime, making most of Herschel requires multi-wavlength approach


![](http://candels.ucolick.org/Images/CANDELS_Circle.jpg)<!-- .element height="20%" width="20%"-->![](http://www.cv.nrao.edu/~mlacy/img/servs_logo.jpg) ![](http://swire.ipac.caltech.edu/swire/images/SWIRE_patch.gif) ![](http://www.cfht.hawaii.edu/Science/CFHTLS/pics.CFHTLS/CFHTLS-Logo.jpg)
![](http://3dhst.research.yale.edu/Data_files/droppedImage.jpg) ![](http://www.sdss.org/wp-content/uploads/2014/05/sdsslogowhite.png)<!-- .element height="20%" width="20%"--> ![](./Slides/assets/KiDSlogo.png)

UKIDSS, DECaLS, DEEP2, ESIS, COSMOS ...

note:
All your favourite surveys form all your favourite telescopes


### The HELP Fields
![](https://github.com/H-E-L-P/H-E-L-P.github.io/blob/master/assets/images/help-fields1.png?raw=true)


### The Masterlist
> A clean list of all sources detected in the optical-mid infrared, with homogenised photometry

Raphael Shirley & Yannick Roehlly


* Decide on best UV/optical/NIR data in given field.
* Collate into single cross matched masterlist.
* Organised into well organised data structure.
* All reproducible and documented.


### Database content

![](./Slides/assets/generic_cols.png) ![](./Slides/assets/perband_cols.png)


###  Reproducible Science and Tools
[![](https://assets-cdn.github.com/images/modules/logos_page/GitHub-Mark.png)<!-- .element height="20%" width="20%"-->](https://github.com/H-E-L-P/XID_plus/)
[![](https://nsls-ii.github.io/_images/jupyter-logo.png)<!-- .element height="20%" width="20%"-->](https://github.com/H-E-L-P/XID_plus/blob/master/docs/notebooks/examples/XID%2Bexample_run_script.ipynb)
[![](https://www.docker.com/sites/default/files/legal/small_v.png)<!-- .element height="22%" width="22%"-->](https://hub.docker.com/r/pdh21/xidplus/)

note:
Yannick, Raphael, Seb, Steven
Pushing for transparent way of working..


### Why Care about FIR emission?
e.g. Dole et al. 2016, Burgarella et al. 2013

![](Slides/assets/Dole_2006.png?raw=true)<!-- .element height="40%" width="40%"--> ![](Slides/assets/Denis_2013.png?raw=true)<!-- .element height="40%" width="40%"-->

note:
* Understand evolution of galaxies
* Understand all SED of galaxies
* Assign IR flux to appropriate sources


### Source Confusion
![](Slides/assets/confusion.gif)<!-- .element height="60%" width="60%"-->

note:
* Now problems with FIR data
* Normal source extraction won't work
* Don't know what or how much source contributes to FIR blob


### List Driven source extraction
Know where sources are so attribute flux to those sources
* XID/DESPHOT: Roseboom et al. 2010, 2012, Wang et al. 2014
* TPHOT: Merlin et al. 2015
* LAMBDAR: Wright et al. 2016:
* Stacking (e.g. Bethermin et al. 2012, Viero et al. 2013 etc)

note:
* Solution is to do list driven approach
* use prior information to build data model, infer model on maps
* All are Maximum likelihood based:
* What does all this mean??
