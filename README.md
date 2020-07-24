# ISMRM Preclinical 
Materials to supplement my 2020 ISMRM educational talk (Clinical vs. Preclinical Data Acquisition, Reconstruction & Translation) on preclinical MRI. 

This is IN PROGRESS (slightly behind schedule -- sorry!) and will be updated soon. 

Experimental design is absolutely key to the accurate interpretation of preclinical MR experiments. This is a vast area of active research, and while there are too many resources to mention directly _everything_ at every level, I think a few brief points need making 

1) Error propagation. 

In MR, and in particular MR spectroscopy, we operate in an SNR-starved regime. Our measurements have errors, and yet it is very rare that their propagation is taken into account properly throughout the analysis. In particular, if you perform function of MR peak amplitudes, say, you are effectively computing functions of a random variable -- and their resulting distribution is _not_ necessarily related to that of the original variables. This point is expanded in detail [here](https://onlinelibrary.wiley.com/doi/full/10.1002/mrm.26615 ), and the particularly keen might like to see a monte-carlo simulation of, say, [the Ernst angle in the heart being imaged once per cardiac cycle, with a plausible range of T1 and TRs](http://caladis.org/compute/?q=acos(exp(-%24tr%2F%24t1))*180%2Fpi&v=tr%3Anorm%2C900%2C250%3Bt1%3Anorm%2C1230%2C200&x=off&n=m&h=fd&a=rad). 

2) Modern statistical methods 
