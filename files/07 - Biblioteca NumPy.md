>**introdução python - Biblioteca NumPy**    
> Repositório: python - Fundamentos  
> GitHub: @gastaldoguilherme
&nbsp;



## Biblioteca NumPy


#### Importando a biblioteca numpy
```python
import numpy as np
```

#### Criando uma matriz unidimensional
```python
mt = np.array([12, 34, 26, 18, 10])
print(mt)
print(type(mt))
```
Resultado:
```
[12 34 26 18 10]
<class 'numpy.ndarray'>
```

#### Criando arrays com tipos específicos
```python
# Criando um array como float de 64 bits
mtfloat = np.array([1, 2, 3], dtype=np.float64)
print(mtfloat)
print(type(mtfloat)

# Criando um array como int32
mtint = np.array([1, 2, 3], dtype=np.int32)
print(mtint)
print(type(mtint)
```
Resultado:
```
[1. 2. 3.]
<class 'numpy.ndarray'>
[1 2 3]
<class 'numpy.ndarray'>
```

#### Mudando o tipo do array
```python
# Transformando tipos de dados de arrays
mtnew = np.array([1.4, 3.6, -5.1, 9.42, 4.999999])
print(mtnew)

# Quando transformamos de float para int os valores são truncados
mtnewint = mtnew.astype(np.int32)
print(mtnewint)
```
Resultado:
```
[ 1.4       3.6      -5.1       9.42      4.999999]
[ 1  3 -5  9  4]
```

#### Conversão de tipos
```python
# Podemos fazer o inverso também
mt5 = np.array([1, 2, 3, 4])
print(mt5)
mt6 = mt5.astype(float)
print(mt6)
```
Resultado:
```
[1 2 3 4]
[1. 2. 3. 4.]
```

#### Matrizes multidimensionais
```python
# Criando uma matriz bidimensional
mt7 = np.array([[7, 2, 23], [12, 27, 4], [5, 34, 23]])
print(mt7)
```
Resultado:
```
[[ 7  2 23]
 [12 27  4]
 [ 5 34 23]]
```

#### Criando arrays vazios tipificados
```python
# "empty" significa que não são inicializados, não que são vazios
vazio = np.empty([3, 2], dtype=int)
print(vazio)
print("-------")

# Criando uma matriz 4x3 com valores zero
zeros = np.zeros([4, 3])
print(zeros)
print("-------")

# Com valores iguais a um
um = np.ones([5, 7])
print(um)
print("-------")

# Criando matriz quadrada com diagonal principal com valores 1 e os outros valores zero
diagonal = np.eye(5)
print(diagonal)
```
Resultado:
```
[[         0 1072693248]
 [         0 1073741824]
 [         0 1074266112]]
-------
[[0. 0. 0.]
 [0. 0. 0.]
 [0. 0. 0.]
 [0. 0. 0.]]
-------
[[1. 1. 1. 1. 1. 1. 1.]
 [1. 1. 1. 1. 1. 1. 1.]
 [1. 1. 1. 1. 1. 1. 1.]
 [1. 1. 1. 1. 1. 1. 1.]
 [1. 1. 1. 1. 1. 1. 1.]]
-------
[[1. 0. 0. 0. 0.]
 [0. 1. 0. 0. 0.]
 [0. 0. 1. 0. 0.]
 [0. 0. 0. 1. 0.]
 [0. 0. 0. 0. 1.]]
```

#### Valores aleatórios
```python
# Valores aleatórios entre zero e um
ale = np.random.random((5))
print(ale)
print("-------")

# Valores aleatórios distribuídos normalmente contendo negativos
ale2 = np.random.randn((5))
print(ale2)
print("-------")

# Valores aleatórios 3x4
ale3 = (10 * np.random.random((3, 4)))
print(ale3)
```
Resultado:
```
[0.30578071 0.44384083 0.03883699 0.53083107 0.35758381]
-------
[ 0.13259578  0.54887523 -1.08384019 -0.42955813 -1.17271359]
-------
[[5.99001794 8.99869821 0.80880142 2.12189234]
 [8.64481223 0.05908113 3.71668918 5.39606774]
 [6.65601744 1.59428705 0.22471724 8.61443986]]
```

#### Gerando números aleatórios com semente
```python
# Outra forma de gerar números aleatórios é usando uma semente
gnr = np.random.default_rng(1)
ale5 = gnr.random(3)
print(gnr)
print(ale5)

# Gerando números inteiros
ale6 = gnr.integers(10, size=(3, 4))
print(ale6)
```
Resultado:
```
Generator(PCG64)
[0.51182162 0.9504637  0.14415961]
[[8 9 2 3]
 [8 4 2 8]
 [2 4 6 5]]
```

#### Removendo repetições
```python
# Remove repetições de um array
j = np.array([11, 12, 13, 14, 15, 16, 17, 12, 13, 11, 18, 19, 20])
j = np.unique(j)
print(j)
```
Resultado:
```
[11 12 13 14 15 16 17 18 19 20]
```

#### Funções específicas
```python
# Criando uma matriz bidimensional
k = np.array([[17, 22, 43], [27, 25, 14], [15, 24, 32]])
# Mostrando a matriz k
print(k)
# Mostrando um elemento específico da matriz k
print(k[0][1])
# Mostrando o tamanho das dimensões da matriz k
print(k.shape)
```
Resultado

:
```
[[17 22 43]
 [27 25 14]
 [15 24 32]]
22
(3, 3)
```

#### Funções matemáticas
```python
# Mostrando o maior valor da matriz k
print(k.max())
# Mostrando o menor valor da matriz k
print(k.min())
# Mostrando a soma dos valores da matriz k
print((k.sum()))
# Mostrando o valor da média dos valores da matriz k
print(k.mean())
# Mostrando o valor do desvio padrão (standard deviation) dos valores da matriz k
print(k.std())
```
Resultado:
```
43
14
219
24.333333333333332
8.615231988880057
```

### Funções Universais em NumPy

Neste exemplo, você verá como as funções universais em NumPy são aplicadas a todos os elementos de um array e seus resultados.

```python
#funções universais, aplicadas a todos os elementos
# Mostra o valor da raiz quadrada de todos elementos
k1 = np.array([1, 4, 9, 16, 25, 36])
print(np.sqrt(k1))
```
Resultado:
```
[1. 2. 3. 4. 5. 6.]
```

```python
# Mostra o valor do exponencial de todos elementos
print(np.exp(k1))
```
Resultado:
```
[2.71828183e+00 5.45981500e+01 8.10308393e+03 8.88611052e+06 7.20048993e+10 4.31123155e+15]
```

### Extração de Elementos

Aqui, você aprenderá a extrair elementos de arrays NumPy.

```python
#extração de elementos
m = np.array([1, 2, 3, 4, 5, 6])
# Mostra o elemento da posição 2
print(m[1])
```
Resultado:
```
2
```

```python
print(m[0:2])
```
Resultado:
```
[1 2]
```

```python
print(m[1:])
```
Resultado:
```
[2 3 4 5 6]
```

```python
print(m[-3:])
```
Resultado:
```
[4 5 6]
```

### Extração de Linhas e Colunas

Aqui, você verá como extrair linhas e colunas de arrays NumPy.

```python
#extração de linhas e colunas
l = np.array([[4, 5], [6, 1], [7, 4]])
print(l)
```
Resultado:
```
[[4 5]
 [6 1]
 [7 4]]
```

```python
l_linha_1 = l[0, :]
print(l_linha_1)
```
Resultado:
```
[4 5]
```

```python
l_linha_2 = l[1, :]
print(l_linha_2)
```
Resultado:
```
[6 1]
```

```python
l_linha_3 = l[2, :]
print(l_linha_3)
```
Resultado:
```
[7 4]
```

```python
#todas as linhas, primeira coluna
l_coluna_1 = l[:, 0]
print(l_coluna_1)
```
Resultado:
```
[4 6 7]
```

```python
#todas as linhas, segunda coluna
l_coluna_2 = l[:, 1]
print(l_coluna_2)
```
Resultado:
```
[5 1 4]
```

### Adição e Multiplicação de Matrizes

Aqui estão exemplos de adição e multiplicação de matrizes em NumPy.

```python
n = np.array([[1, 2], [3, 4]])
o = np.array([[1, 1], [1, 1]])

res1 = n + o
print(res1)
```
Resultado:
```
[[2 3]
 [4 5]]
```

```python
# Multiplicação de Matrizes - Produto Matricial
res2 = n @ o
print(res2)
```
Resultado:
```
[[3 3]
 [7 7]]
```

```python
# Produto de Hadamard (também conhecido como produto elemento a elemento)
res2 = n * o
print(res2)
```
Resultado:
```
[[1 2]
 [3 4]]
```

```python
# #adição de matrizes com dimensões diferentes:
p = np.array([[1, 2], [3, 4], [5, 6]])
q = np.array([[2, 1]])
print(p + q)
```
&nbsp;
Obs: O NumPy utiliza um conceito chamado "broadcasting" (transmissão ou difusão, em tradução livre) para realizar operações entre matrizes de diferentes formas. O broadcasting é uma técnica que permite ao NumPy realizar operações em matrizes que não possuem as mesmas dimensões, desde que elas satisfaçam algumas regras específicas.
&nbsp;

Resultado:
```
[[3 3]
 [5 5]
 [7 7]]
```

### Transposição de Matrizes

Aqui você verá como realizar a transposição de matrizes em NumPy.

```python
# transposição, rearranja um conjunto de 15 elementos de 0 a 14
# em 3 linhas e 5 colunas.
f = np.arange(15).reshape((3, 5))
# mostra a matriz transposta entre linha e coluna
print(f)
```
Resultado:
```
[[ 0  1  2  3  4]
 [ 5  6  7  8  9]
 [10 11 12 13 14]]
```

```python
s = f.T
print(s)
```
Resultado:
```
[[ 0  5 10]
 [ 1  6 11]
 [ 2  7 12]
 [ 3  8 13]
 [ 4  9 14]]
```

### Expressões Lógicas

Neste exemplo, você verá como usar expressões lógicas em NumPy.

```python
# expressões lógicas
# usando where
# criando uma matriz com valores aleatórios positivos e negativos
v = np.random.randn(4, 4)
print(v)
```
Resultado:
```
[[-0.49656349 -0.15183751 -0.70899678  0.95764648]
 [-0.79642058  1.24283349 -0.24763993  0.61061306]
 [-1.00554832 -0.55418092 -0.00011998  0.36623806]
 [-0.74694888 -2.95980339 -1.09055013  0.03648647]]
```

```python
# criando uma matriz com valores booleanos com base no array v
x = (v > 0)
print(x)
```
Resultado:
```
[[False False False  True]
 [False  True False  True]
 [False False False  True]
 [False False False  True]]
```

```python
# criando uma matriz com valores -1 e 1 com base nos valores do array x
z = np.where(x > 0, 1, -1)
print(z)
```
Resultado:
```
[[-1 -1 -1  1]
 [-1  1 -1  1]
 [-1 -1 -1  1]
 [-1 -1 -1  1]]


```




&nbsp;

<div align="center">
   
[Retornar ao índice](/README.md)

</div>