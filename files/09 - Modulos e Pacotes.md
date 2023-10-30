>**introdução python - Módulos e Pacotes**    
> Repositório: python - Fundamentos  
> GitHub: @gastaldoguilherme
&nbsp;



## Módulos e Pacotes

Neste exemplo, demonstra-se como importar módulos e funções de módulos no Python e como usar essas funções para calcular a média e a mediana de uma lista de números.

### Importando um Módulo e Usando um Apelido

```python
import statistics
z = [10, 20, 30, 40]
x = statistics.mean(z)
y = statistics.median(z)
print(x)
print(y)
```

**Resultado:**
```
25
25.0
```

### Importando um Módulo com um Apelido

```python
import statistics as est
z = [10, 20, 30, 40]
x = est.mean(z)
y = est.median(z)
print(x)
print(y)
```

**Resultado:**
```
25
25.0
```

### Importando Funções Específicas de um Módulo

```python
from statistics import mean, median
z = [10, 20, 30, 40]
x = mean(z)
y = median(z)
print(x)
print(y)
```

**Resultado:**
```
25
25.0
```

### Importando Todas as Funções de um Módulo

```python
from statistics import *
z = [10, 20, 30, 40]
x = mean(z)
y = median(z)
print(x)
print(y)
```

**Resultado:**
```
25
25.0
```

&nbsp;

<div align="center">
   
[Retornar ao índice](/README.md)

</div>