# Scripts de scilab

```
Tamaño de la matriz: 3 
 

Matriz C:
   22.   34.   85.   7. 
   76.   67.   69.   57.
   1.    63.   88.   67.

   1.   0.   0.  -0.3749055
   0.   1.   0.   1.855713 
   0.   0.   1.  -0.5628979
```

Uso de scilab para análisis numerico

## Software
[scilab 6.1.1](https://www.scilab.org/download/scilab-6.1.1)

## Proyectos
### [Raices de numeros](https://github.com/adnksharp/sSqrt/blob/base/sqrt.sce)
Calcula las raices de un numero usando iteraciones:

    sqroot_i = (sqroot_i + (x / sqroot_(i-1)) / 2

### [Radio y angulo](https://github.com/adnksharp/sTraxy)
Calcula el radio y el angulo de un circulo usando coordenadas cartesianas usando el teorema de pitagoras y la funcion **atan**

```scilab
sqroot(x^2 + y^2)
atan(y/x) * 180 / %pi
```

### [1 / (i^x)](https://github.com/adnksharp/sInfinite)
Calculo de la funcion `1/(i^x)` que tiende a `%pi^n/90`

### [Factorial](https://github.com/adnksharp/sFactorial)
Calcula el factorial de un numero usando iteraciones:

    x! = x! * i

### [Función Exponencial](https://github.com/adnksharp/sSxponential)
Calrulo de la función exponencial usando iteraciones:

```
sxponential = sxponential + ((x^i) / (i!))
```

### [Funciones trigonometricas](https://github.com/adnksharp/sTrigonometric)
Calcula las funciones trigonometricas usando iteraciones:

#### cos(x)
```
1 +/- x^(i)/(2i!)
```

#### sin(x)
```
x +/- x^(i)/((2i+1)!)
```

### [Formula general](https://github.com/adnksharp/sECq)
Solucion de ecuaciones cuadraticas ingresando los coeficientes de la ecuacion:
    
    a*x^2 + b*x + c = 0

### [Formula de Stefan-Boltzmann](https://github.com/adnksharp/sS-B)
Calcula la formula de Stefan-Boltzmann:

```
H=AeσT^4
```

### Metodos para obtener raices de ecuaciones
#### [Biseccion](https://github.com/adnksharp/sIbisection)
Calculo de la raiz de una ecuacion usando el metodo de biseccion:

```
x_i = (x_l - x_u) / 2
```

#### [Convergencia](https://github.com/adnksharp/sConvergence)
Calculo de la raiz de una ecuacion usando el metodo de convergencia:

``` python
f = f(x_1) - f(x_2) or f(x_1) + f(x_2)
```

#### [Secante](https://github.com/adnksharp/sSecant)
Calculo de la raiz de una ecuacion usando el metodo de secante:

```
f'(x_n) = (f(x_n-1) - f(x_n)) / (x_n-1 - x_n)
```

#### [Newton-Raphson](https://github.com/adnksharp/sNR)
Calculo de la raiz de una ecuacion usando el metodo de Newton-Raphson:

```
x_n+1 = x_n - f(x_n)/f'(x_n)
```

#### [Müller](https://github.com/adnksharp/sMuller)
Calculo de la raiz de una ecuacion usando el metodo de Muller:

```
δ = ( f[2] - f[0] ) / ( f[1] - f[0] )
Δx_0 = x_1 - x_0
Δx_1 = x_2 - x_1

a = (δ - δ_0) / (Δx_0 + Δx_1)
b = a * Δx_1 / δ
c = f[2]

x_n+1 = x_n + (-2c)/ (b +/- sqrt(b^2-4ac))
```

### [Valores de matrices](https://github.com/adnksharp/sFarrays)
Obtener valores de una matriz:
    
- Promedio
- Maximo
- Minimo
- Raiz cuadrada

#### [Solucion de matrices](https://github.com/adnksharp/sFmatrix)
- Determinante: Calculo del determinante de una matriz usando la funcion **det**.

- Cramer: Resolver matrices usando el metodo de Cramer (obteniendo el determinante de la matriz **x** y de la matriz con los valores sustituidos por el vector **y**)

- Gauss-Jordan: Resolver matrices usando el metodo de Gauss-Jordan

#### [Metodo de burbuja](https://github.com/adnksharp/sObubble/blob/base/bubble.sce)
Ordena un arreglo de numeros usando el metodo de burbuja:

```
eval_i,j < eval_k,l
aux = eval_i,j
eval_i,j = eval_k,l
eval_k,l = aux
```
### [Máximos y mínimos de una función](https://github.com/adnksharp/sO1d)
Uso del metodo de Newton para encontrar el máximo de una función:

```
x_i+1 = x_i - f'(x_i) / f''(x_i)
```

## Ejemplos
### [Prestamo](https://github.com/adnksharp/sPay)
Simulación de un prestamo tomando en cuenta el prestamo, la tasa de interes y el numero de pagos.

### [Calificaciones](https://github.com/adnksharp/sRating)
Calcula la calificacion de una persona de ZZ, F a A y 0 a 100 tomando en cuenta las unidades de la materia, el porcentaje de los rubros a calificar y la calificacion de cada rubro.

## Referencias
[Scilab](https://help.scilab.org/docs/6.1.1/en_US/index.html)
