Meistens ist die Wahrscheinlichkeitsdichte nicht bekannt. Typ der Verteilung (Poisson, Binomial,...) schon, Parameter nicht bekannt.

Schätzung des wahren Werts $\lambda$ durch $\hat\lambda$
Muss folgende Eigenschaften erfüllen:
$$E[\hat\lambda] = \lambda$$$$\lim_{N \to \infty} \hat\lambda(X_1, ..., X_N) = \lambda$$
## Erwartungswert: 
Finde $\bar x$ mit $E[\bar x]=\mu$

$$\bar x = \frac{1}{N} \sum_{i=1}^N X_i$$
``` python
x_bar= np.sum(x)/np.size(x)
```

Wobei x ein array mit Werten (z.B. Normalverteilung)

# Varianz:
$$Var[\bar x] = \frac{1}{N^2} \sum_{i=1}^N Var[X_i] = \frac{\sigma^2}{N}$$

$$V = \frac{1}{N-1} \sum_{i=1}^N (X_i - \bar x)^2$$
