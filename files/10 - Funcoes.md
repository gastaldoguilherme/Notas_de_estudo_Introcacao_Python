>**introdução python - Funções**    
> Repositório: python - Fundamentos  
> GitHub: @gastaldoguilherme
&nbsp;


## Funções

Neste exemplo, demonstra-se como criar funções em Python, funções com parâmetros, funções com retorno e funções com valores padrão (default). Também é mostrado como usar funções em Python para realizar operações específicas.

### Função Sem Parâmetros

```python
def imprime():
    print("esta é uma função")

imprime()
```

**Resultado:**
```
esta é uma função
```

### Função com Parâmetro

```python
def imprime(n):
    print(n)

imprime("Impressão deste texto")
```

**Resultado:**
```
Impressão deste texto
```

### Função com Retorno

```python
def potencia(n):
    return n * n

x = potencia(3)
print(x)
```

**Resultado:**
```
9
```

### Função com Valor Padrão (Default)

```python
def intervalo(inic=1, fim=10):
    for n in range(inic, fim+1):
        print(n)

x = intervalo(1, 10)
y = intervalo()
```

**Resultado:**
```
1
2
3
4
5
6
7
8
9
10
1
2
3
4
5
6
7
8
9
10
```

### Função com Valor Padrão (Default) Modificado

```python
def intervalo(inic=0, fim=5):
    for n in range(inic, fim):
        print(n)

x = intervalo()
```

**Resultado:**
```
0
1
2
3
4
```

### Função com Retorno

```python
def potencia(n):
    return pow(n, 2)

x = potencia(100)
print(x)
```

**Resultado:**
```
10000
```



&nbsp;

<div align="center">
   
[Retornar ao índice](/README.md)

</div>