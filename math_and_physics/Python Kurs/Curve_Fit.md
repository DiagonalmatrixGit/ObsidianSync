Finde die Parameter einer Funktion f anhand der Datenpunkte (x,y) mit Fehler dy:

``` python
def f(x,a,b):               #definiere die Basisfunktion
    return a*x**2+b*x+c

pOpt, pCov = curve_fit(f, x, y, sigma=dy, absolute_sigma=True)
print(pOpt)
```

`pOpt erzeugt einen Array der Paramater von f, hier: [a,b,c] `
`pCov erzeugt die Kovarianzmatrix`