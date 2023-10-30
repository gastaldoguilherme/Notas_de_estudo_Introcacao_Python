>**introdução python - Listas**    
> Repositório: python - Fundamentos  
> GitHub: @gastaldoguilherme
&nbsp;


## Listas

### Formas de Criar Listas

```python
lst = [1, 2, 3, 4, 5]
print(lst)
```

**Resultado:**
```
[1, 2, 3, 4, 5]
```

### Listas com Diferentes Tipos de Dados

```python
lst2 = [1, 2, 3, "4", True]
print(lst2)
```

**Resultado:**
```
[1, 2, 3, '4', True]
```

### Lista Contendo Outras Listas

```python
lst3 = [12, [1, 2, 3, 4, 5], "a"]
print(lst3)
```

**Resultado:**
```
[12, [1, 2, 3, 4, 5], 'a']
```

### Criando uma Lista com `range`

```python
lst4 = list(range(0, 10))
print(lst4)
```

**Resultado:**
```
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
```

### Comprimento da Lista

```python
print(len(lst))
```

**Resultado:**
```
5
```

### Acessando Elementos da Lista

```python
print(lst[0])
print(lst3[1])
lst[0] = 4
print(lst)
```

**Resultado:**
```
1
[1, 2, 3, 4, 5]
[4, 2, 3, 4, 5]
```

### Percorrendo uma Lista

```python
for n in range(0, len(lst4)):
    print(lst4[n] + 1)
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
```


&nbsp;

<div align="center">
   
[Retornar ao índice](/README.md)

</div>