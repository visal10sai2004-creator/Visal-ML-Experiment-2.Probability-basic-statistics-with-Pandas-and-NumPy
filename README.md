## Experiment-2.Probability & basic statistics with Pandas and NumPy

## AIM:

 Compute descriptive statistics and empirical probabilities; generate samples from distributions.

## ALGORITHM :
 
 Use pandas.Series for statistics; numpy.random for sampling

## THEORY:
 
 Descriptive statistics and sampling basics used throughout ML

 ## PROGRAM:

```

import numpy as np
import pandas as pd
heights=np.array([160,165,170,175,180,155,168,172,169,158])
s=pd.Series(heights)
print("mean:",s.mean())
print("median:",s.median())
print("std dev:",round(s.std(),3))
print("variance:",round(s.var(),3))
print("P(height > 170):",(s>170).mean())
sample=np.random.normal(loc=s.mean(),scale=s.std(),size=100)
print("random sample(10)from normal around mean:",np.round(sample,3))

```

## OUTPUT:

```

mean: 167.2
median: 168.5
std dev: 7.815
variance: 61.067
P(height > 170): 0.3
random sample(10)from normal around mean: [161.323 179.73  163.495 167.305 171.072 167.617 168.338 152.295 161.61
 162.787 161.884 163.395 175.219 156.077 152.308 166.37  160.744 175.681
 153.012 177.659 162.597 155.786 148.646 177.635 165.224 166.477 162.145
 167.922 168.616 173.593 170.654 175.768 165.159 164.931 167.184 168.64
 159.289 165.254 171.612 157.006 163.668 162.847 162.512 171.454 167.74
 154.785 160.4   176.176 167.003 161.669 182.146 163.483 161.284 173.34
 157.561 154.838 160.467 177.096 156.907 170.73  171.825 168.368 164.88
 163.603 168.917 165.204 177.102 171.116 168.689 155.593 150.905 179.376
 166.57  159.656 162.115 167.08  161.809 172.43  158.966 170.737 160.332
 163.146 153.089 166.817 169.367 168.733 176.731 187.605 160.305 167.124
 177.59  156.993 166.933 171.231 161.87  171.972 159.047 165.825 161.061
 160.914]

```

## RESULT:
 
 Students learn central tendency, spread, and simple empirical probability estimation.
