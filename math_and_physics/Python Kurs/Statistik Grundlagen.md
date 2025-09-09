Zufallsvariable $X$ Menge der möglichen Ergebnisse.
Wahrscheinlichkeit des Ergebnisses $x$: $P(X=x)$

|                |             Discrete              |                      Continuous                       |
| :------------- | :-------------------------------: | :---------------------------------------------------: |
| Beschreibung   |    Gewichte $$w_x = P(X = x)$$    | Dichte $$\rho(x) = \frac{P(x \le X \le x + dx)}{dx}$$ |
| Normierung     |    $$\sum_{x \in M} w_x = 1$$     |               $$\int_M \rho(x) dx = 1$$               |
| Erwartungswert | $$\mu=E[X]=\sum_{x \in M} x w_x$$ |            $$E[X] = \int_M x \rho(x) dx$$             |
| Varianz        |   $$Var[X] = E[(X - E[X])^2]$$    |             $$Var[X] = E[(X - E[X])^2]$$              |
| Bsp            |         Würfelergebnisse          |                                                       |
$$
\sigma^2=Var[X]
$$
Wahrscheinlichkeitsdichte $\rho(x)$:
``` python
rho = stat.norm.pdf(x)
```

$$
F(x)=P(X \leq x)
$$
``` python
F = stat.norm.cdf(x)
```

$$
\rho(x)=\frac{dF}{dx}
$$
``` python
dF_dx = np.diff(F)/np.diff(x)
```
$$
F(x)=\int_{-\infty}^{x} \rho(x)dx
$$


