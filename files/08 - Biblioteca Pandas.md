>**introdução python - Biblioteca Pandas**    
> Repositório: python - Fundamentos  
> GitHub: @gastaldoguilherme
&nbsp;

## Biblioteca Pandas

A biblioteca Pandas é amplamente utilizada para manipulação e análise de dados em Python. Abaixo, estão algumas das operações comuns realizadas com Pandas, juntamente com os resultados de cada operação:

### Carregando um Arquivo CSV

```python
import pandas as pd
dados = pd.read_csv("Credit.csv")
```

### Formato do DataFrame

```python
dados.shape
```


### Resumo Estatístico de Colunas Numéricas

```python
dados.describe()
```

### Primeiros Registros com Parâmetros

```python
dados.head(5)
```

### Últimos Registros com Parâmetros

```python
dados.tail(5)
```

### Filtrando por Nome da Coluna

```python
dados[["duration"]]
```

### Filtrando Linhas por Índice

```python
dados.loc[1:3]
```

### Selecionando Linhas 1 e 3

Selecionar linhas específicas de um DataFrame em pandas. Ela permite selecionar as linhas com base em seus rótulos de índice. 
No exemplo dados.loc[[1,3]], você está selecionando as linhas cujos rótulos de índice são 1 e 3.

```python
dados.loc[[1,3]]
```

### Filtrando com Condição (Exemplo: "purpose" igual a "radio/tv")

```python
dados.loc[dados['purpose'] == "radio/tv"]
```

### Filtrando com Outra Condição (Exemplo: "credit_amount" maior que 18000)

```python
dados.loc[dados['credit_amount'] > 18000]
```

### Atribuindo Resultado a uma Variável e Criando Outro DataFrame

```python
credito2 = dados.loc[dados['credit_amount'] > 18000]
print(credito2)
```

### Definindo Apenas Algumas Colunas do DataFrame

```python
credito3 = dados[['checking_status', 'duration']].loc[dados['credit_amount'] > 18000]
print(credito3)
```

### Trabalhando com Séries (Colunas)

#### Criando uma Série a partir de uma Lista

```python
s1 = pd.Series([2, 5, 3, 34, 54, 23, 1, 16])
print(s1)
```

#### Criando uma Série a partir de um Array do Numpy

```python
import numpy as np
array1 = np.array([2, 5, 3, 34, 54, 23, 1, 16])
s2 = pd.Series(array1)
print(s2)
```

#### Criando uma Série a partir do DataFrame

```python
s3 = dados['purpose']
print(s3)
```

**Tipo de s3:**
```
<class 'pandas.core.series.Series'>
```

#### Diferença entre Série e DataFrame

```python
d4 = dados[['purpose']]
type(d4)
```

**Tipo de d4:**
```
<class 'pandas.core.frame.DataFrame'>
```

### Renomeando Colunas do DataFrame

Renomear colunas, mas a alteração não é persistida:

```python
dados.rename(columns={"duration":"duração", "purpose":"propósito"})
```

### Persistindo a Alteração no DataFrame

```python
dados.rename(columns={"duration":"duração", "purpose":"propósito"}, inplace=True)
```

### Excluindo uma Coluna do DataFrame

```python
dados.drop('checking_status', axis=1, inplace=True)
print(dados)
```

### Verificando a Saída após Excluir a Coluna

### Verificando Dados Nulos no DataFrame

```python
dados.isnull()
```

### Verificando a Quantidade de Dados Nulos por Coluna

```python
dados.isnull().sum()
```

### Removendo Linhas com Valores Nulos

```python
dados.dropna()
```

### Preenchendo Dados Faltantes em uma Coluna

```python
dados['duração'].fillna(0, inplace=True)
```

### Selecionando Parte do DataFrame Usando "iloc"

Selecionar dados em um DataFrame com base em sua posição numérica, em vez de rótulos de índice ou coluna:

```python
dados.iloc[0:3, 0:5]
```

```python
dados.iloc[[0, 1, 2, 3, 7], 0:5]
```




&nbsp;

<div align="center">
   
[Retornar ao índice](/README.md)

</div>