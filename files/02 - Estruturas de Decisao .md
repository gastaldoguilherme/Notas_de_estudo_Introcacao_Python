>**introdução python - Estruturas de Decisão**    
> Repositório: python - Fundamentos  
> GitHub: @gastaldoguilherme
&nbsp;

## Estruturas de Decisao

#### Verificação de Notas

#### Caso 1: Nota maior ou igual a 7
```python
nota = 7
if nota >= 7:
    print("Aprovado")
    print("Parabéns!")
else:
    print("Reprovado")
```

**Resultado:**
```
Aprovado
Parabéns!
```

#### Caso 2: Nota menor que 7
```python
# Só mudar o valor da variável
nota = 5
if nota >= 7:
    print("Aprovado")
else:
    print("Reprovado")
```

**Resultado:**
```
Reprovado
```

#### Caso 3: Testando com diferentes notas
```python
# Testar com 4,5 e 7
nota = 4.000000000000001
if nota <= 4:
    print("Reprovado")
elif nota > 4 and nota <= 6:
    print("Exame")
else:
    print("Aprovado")
```

**Resultado:**
```
Exame
```



&nbsp;

<div align="center">
   
[Retornar ao índice](/README.md)

</div>