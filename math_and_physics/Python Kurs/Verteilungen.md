# Normalverteilung
$$\rho(x |\, \mu, \sigma) = \frac{1}{\sqrt{2\pi\sigma^2}} \cdot \exp{\left(-\frac{(x-\mu)^2}{2\sigma^2}\right)}$$
``` python
mu = 1         #Erwarungswert
sigma = 0.5    #Varianz
N = 1000       #Stichprobe

x = np.random.normal(loc=mu, scale=sigma, size=N) 
```

# Bernoulli
 two possible outcomes (*1* and *0*)
$$P(X = 1) = p$$
$$P(X = 0) = 1 - p$$
``` python
n = 1         
pTrue = 0.3   
size = 1000       

x = np.random.binomial(n, pTrue, size=size)
```

# Binomial


Erwartungswert:
$E[X]=...= n \cdot p$

