
``` python
x, y, dy = np.loadtxt("DATENSET.txt", unpack=True)
```

Bestimme Daten via [Curve Fit](Curve_Fit).

Chi Quadrat $\chi ^2$ für eine Funktion mit zwei Parametern:

``` python
chi2 = np.sum(((y-f(x, pOpt[0], pOpt[1]))/dy)**2)
```

Chi Quadrat reduziert:

$$
\chi ^2_{red}=\frac{\chi ^2}v
$$
 Mit dem Freiheitsgrad: $v=N-k$ 
$N$ = Anzahl der Datenpunkte (`size(x)`)
$k$ = Anzahl Parameter von f(x, a, b, ...) 


