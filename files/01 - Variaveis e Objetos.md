>**introdução python - Variáveis e Objetos**    
> Repositório: python - Fundamentos  
> GitHub: @gastaldoguilherme
&nbsp;


## Variáveis e Objetos

### Cria variável do tipo inteiro
```python
x = 1
print(x)
```
Resultado: `1`

### Cria variável do tipo float
```python
y = 3.13
print(y)
```
Resultado: `3.13`

### Cria variável do tipo string
```python
m = "Python"
m = 'Python'
print(m)
```
Resultado: `Python`

### Cria variável do tipo lógica
```python
w = True  
y = False
print(y)
```
Resultado: `False`

### Calculadora
```python
x = 10
y = 20
z = 100
w = (x + y) * z / 100
print(w)
```
Resultado: `30.0`

### Exibir texto no console
```python
print("Este texto será impresso no console")
print(x)
print("Texto e duas variáveis: ", x, ", ", z)
```
Resultado:
```
Este texto será impresso no console
10
Texto e duas variáveis:  10 ,  100
```

### Verificar tipo
```python
print(type(x))
print(type(m))
```
Resultado:
```
<class 'int'>
<class 'str'>
```

### Entrada de dados
```python
print("Informe o valor: ")
i = input()
# Mostra tipo string
print(type(i))
```
```
Resultado: i= 'python' ou i=10
```
Informe o valor: 
```
 python ou 10

<class 'str'>

```

### Entrada de valor com mensagem separada e junto
```python
print("Informe o valor: ")
i = input()
# ou
i = input("Informe o valor: ")
```
Resultado:
```
Informe o valor: 
 10
Informe o valor:  10

```

### Conversão de valores
#### Para inteiro
```python
var = input("Informe o valor: ")
print(type(var))
var = int(var)
print(type(var))
```
Resultado:
```
Informe o valor:  10

<class 'str'>
<class 'int'>

```


#### Para float
```python
var = input("Informe o valor: ")
print(type(var))
var = float(var)
print(type(var))
```
Resultado:
```
Informe o valor:  10.25

<class 'str'>
<class 'float'>

```


### Comentários
```python
# Este texto é um comentário
X = 10  # a partir daqui é um comentário
```
&nbsp;

<div align="center">
   
[Retornar ao índice](/README.md)

</div>