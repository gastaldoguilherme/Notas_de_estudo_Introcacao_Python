>**introdução python - Dicionários, Sets e Tuplas**    
> Repositório: python - Fundamentos  
> GitHub: @gastaldoguilherme
&nbsp;



# Dicionários, Sets e Tuplas

## Dicionários:
```python
# Dicionários: estrutura chave/valor
Notas = {'João': 6.0, 'Maria': 8.0, 'Pedro': 6.5}
print(Notas)
```

**Resultado:**
```
{'João': 6.0, 'Maria': 8.0, 'Pedro': 6.5}
```

#### Acessando um valor no dicionário:
```python
print(Notas['João'])
```

**Resultado:**
```
6.0
```

#### Listando todas as chaves do dicionário:
```python
Notas.keys()
```

**Resultado:**
```
dict_keys(['João', 'Maria', 'Pedro'])
```

#### Listando todos os valores do dicionário:
```python
Notas.values()
```

**Resultado:**
```
dict_values([6.0, 8.0, 6.5])
```

#### Verificando a existência de uma chave no dicionário:
```python
print('João' in Notas)
print('Fernando' in Notas)
```

**Resultado:**
```
True
False
```

#### Removendo um elemento do dicionário:
```python
del Notas['João']
print(Notas)
```

**Resultado:**
```
{'Maria': 8.0, 'Pedro': 6.5}
```

#### Adicionando um elemento ao dicionário:
```python
Notas['Ana'] = 9
print(Notas)
```

**Resultado:**
```
{'Maria': 8.0, 'Pedro': 6.5, 'Ana': 9}
```

#### Buscando um valor no dicionário com um valor padrão se não encontrado:
```python
Notas.get('Geraldo', "Não encontrado!")
```

**Resultado:**
```
'Não encontrado!'
```

## Sets:
```python
# Sets são conjuntos não ordenados de elementos não repetidos
bigdata = {'Spark', 'Hive', 'Sqoop'}
print(bigdata)
```

**Resultado:**
```
{'Spark', 'Hive', 'Sqoop'}
```

#### Verificando a existência de um elemento no set:
```python
print('Spark' in bigdata)
```

**Resultado:**
```
True
```

#### Adicionando um elemento ao set:
```python
bigdata.add('Hadoop')
bigdata
```

**Resultado:**
```
{'Hadoop', 'Hive', 'Spark', 'Sqoop'}
```

#### Obtendo o número de elementos em um set:
```python
print(len(bigdata))
```

**Resultado:**
```
4
```

## Tuplas:
```python
# Tuplas são listas que não podem ser alteradas
# Listas usam [], tuplas usam ()
tupla = (1, 2, 3, 4, 5, 6, 7)
tupla
```

**Resultado:**
```
(1, 2, 3, 4, 5, 6, 7)
```

#### Acessando um elemento em uma tupla:
```python
tupla[4]
```

**Resultado:**
```
5
```

#### Dicionários com Tuplas:
```python
# Dicionários em que cada posição recebe uma tupla
dic2 = {(0, 1): 0, (1, 2): 1, (2, 3): 2, (3, 4): 3, (4, 5): 4, (5, 6): 5, (6, 7): 6, (7, 8): 7, (8, 9): 8, (9, 10): 9}
dic2
```

**Resultado:**
```
{(0, 1): 0, (1, 2): 1, (2, 3): 2, (3, 4): 3, (4, 5): 4, (5, 6): 5, (6, 7): 6, (7, 8): 7, (8, 9): 8, (9, 10): 9}
```

#### Tipos de Dados:
```python
print(type(Notas))
print(type(bigdata))
print(type(tupla))
```

**Resultado:**
```
<class 'dict'>
<class 'set'>
<class 'tuple'>
```

Neste código, são apresentados exemplos de uso de dicionários, sets e tuplas em Python, juntamente com os resultados para cada seção.

&nbsp;

<div align="center">
   
[Retornar ao índice](/README.md)

</div>