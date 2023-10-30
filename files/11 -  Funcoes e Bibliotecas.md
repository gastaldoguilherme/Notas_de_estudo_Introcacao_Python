>**introdução python - Funções e Bibliotecas**    
> Repositório: python - Fundamentos  
> GitHub: @gastaldoguilherme
&nbsp;

## Funções e Bibliotecas

Neste exemplo, são demonstradas funções internas do Python, bem como o uso da biblioteca `statistics` para cálculos estatísticos em uma lista de números. Também é apresentado o uso da biblioteca `NumPy` para criar uma matriz de números aleatórios.



### Funções Internas do Python

```python
# Funções internas do Python
print(abs(-200))
lst = [1, 2, 30, 30, 45]
print("Maior valor:", max(lst))
print("Menor valor:", min(lst))
print("Soma:", sum(lst))
print("Arredondamento:", round(2.34567, 2))
```

**Resultado:**
```
200
Maior valor: 45
Menor valor: 1
Soma: 108
Arredondamento: 2.35
```

### Biblioteca `statistics`

```python
# Utilizando a biblioteca statistics
from statistics import *

print("Média:", mean(lst))
print("Mediana:", median(lst))
print("Moda:", mode(lst))
```

**Resultado:**
```
Média: 21.6
Mediana: 30
Moda: 30
```

### Desvio Padrão da Amostra

```python
# Desvio padrão da amostra
print("Desvio padrão:", stdev(lst))
```

**Resultado:**
```
Desvio padrão: 14.945651284468493
```

### Variância da Amostra

```python
# Variância da amostra
print("Variância:", variance(lst))
```

**Resultado:**
```
Variância: 223.3
```

### Biblioteca NumPy

```python
# Utilizando a biblioteca NumPy
from numpy import *
a = random.random((8, 8))
print(type(a))
print(a)
```

**Resultado:**
```
<class 'numpy.ndarray'>
[[0.97490387 0.88822963 0.86411804 0.14179559 0.82575673 0.48590948
  0.19677659 0.86111938]
 [0.25075222 0.27195775 0.22526215 0.68896645 0.84474421 0.27474304
  0.65082984 0.36453589]
 [0.91591494 0.76856439 0.38907314 0.58734664 0.87160662 0.45345686
  0.75975618 0.683481  ]
 [0.23566226 0.07369836 0.13698271 0.07198049 0.99699192 0.29696899
  0.72765902 0.8996604 ]
 [0.28505791 0.39373498 0.70737709 0.21583268 0.18394029 0.14482874
  0.90022989 0.30024339]
 [0.33225468 0.2708233  0.03827984 0.37045154 0.81824053 0.85206117
  0.59739267 0.46147024]
 [0.98955468 0.09716082 0.65591102 0.91381965 0.30110651 0.59870803
  0.10237334 0.70610587]
 [0.50243794 0.91998159 0.58384016 0.14048444 0.06240177 0.97511771
  0.32452567 0.83415709]]
```



&nbsp;

<div align="center">
   
[Retornar ao índice](/README.md)

</div>