>**introdução python - Estruturas de Repetição**    
> Repositório: python - Fundamentos  
> GitHub: @gastaldoguilherme
&nbsp;



## Estruturas de Repetição

#### Exemplo com `while`:
```python
# exemplo com while
count = 1
while count <= 5:
    print(count)
    count += 1
```

**Resultado:**
```
1
2
3
4
5
```

#### Exemplo com `for` e `range`:
```python
# for normal
for n in range(0, 10, 1):
    print(n + 1)

for n in range(1, 11):
    print(n)
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

#### Exemplo com `for` decrescente:
```python
# for decrescente
for n in range(10, 0, -1):
    print(n)
```

**Resultado:**
```
10
9
8
7
6
5
4
3
2
1
```

#### Exemplo com `break`:
```python
# exemplo com break
# vai parar no 3, pois o break está antes do print
for n in range(0, 10):
    if n == 4:
        break
    print(n)
```

**Resultado:**
```
0
1
2
3
```

#### Exemplo com `continue`:
```python
# exemplo com continue
# vai pular o número 4
for n in range(0, 10):
    if n == 4:
        continue
    print(n)
```

**Resultado:**
```
0
1
2
3
5
6
7
8
9
```

Neste código, são demonstrados exemplos de estruturas de repetição `while` e `for`, bem como o uso de `range`. Também são apresentados exemplos de uso de `break` e `continue` dentro de loops. Os resultados para cada caso estão incluídos.

&nbsp;

<div align="center">
   
[Retornar ao índice](/README.md)

</div>