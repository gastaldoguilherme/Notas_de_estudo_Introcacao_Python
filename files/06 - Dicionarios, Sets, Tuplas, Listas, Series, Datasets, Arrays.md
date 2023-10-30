>**introdução python - Dicionários, Sets, Tuplas, Listas, Séries, Datasets, Arrays**    
> Repositório: python - Fundamentos  
> GitHub: @gastaldoguilherme
&nbsp;

Em Python, cada uma dessas estruturas de dados tem um propósito específico:

1. **Dicionários (Dictionaries):** Dicionários são estruturas de dados que representam uma coleção de pares chave-valor. Cada elemento é composto por uma chave única associada a um valor correspondente. Dicionários são muito eficientes para buscar valores por chave. Eles são definidos com chaves `{}`.

   Exemplo:
   ```python
   dicionario = {'nome': 'Alice', 'idade': 25, 'cidade': 'Nova York'}
   ```

2. **Sets (Conjuntos):** Sets são coleções não ordenadas de elementos únicos. Eles são usados para armazenar valores distintos e não possuem índices ou chaves associados. Conjuntos são definidos com chaves `{}` ou a função `set()`.

   Exemplo:
   ```python
   conjunto = {1, 2, 3, 4, 5}
   ```

3. **Tuplas (Tuples):** Tuplas são sequências ordenadas e imutáveis de elementos. Eles são usados para armazenar coleções de valores que não devem ser modificados. Tuplas são definidas usando parênteses `()`.

   Exemplo:
   ```python
   tupla = (1, 2, 3, 'abc', 3.14)
   ```

4. **Listas (Lists):** Listas são coleções ordenadas de elementos que podem ser modificados. Elas são usadas para armazenar valores em uma ordem específica e podem conter elementos de tipos diferentes. Listas são definidas com colchetes `[]`.

   Exemplo:
   ```python
   lista = [10, 20, 30, 'abc', 3.14]
   ```

5. **Séries (Pandas Series):** As séries são uma estrutura de dados unidimensional fornecida pela biblioteca Pandas. Elas são semelhantes a listas ou arrays NumPy, mas também têm rótulos para indexação, tornando-as ideais para análise de dados.

   Exemplo (usando Pandas):
   ```python
   import pandas as pd
   serie = pd.Series([10, 20, 30, 40])
   ```

6. **Datasets:** O termo "dataset" se refere a um conjunto de dados que geralmente contém várias observações ou registros, com múltiplas variáveis ou atributos. Datasets podem ser armazenados em formatos como CSV, Excel, SQL, JSON, etc., e são frequentemente manipulados com bibliotecas como Pandas para análise de dados.

7. **Arrays:** Arrays são estruturas de dados multidimensionais que armazenam elementos de um tipo de dados comum. Em Python, a biblioteca NumPy fornece suporte para arrays multidimensionais eficientes, que são frequentemente usados em cálculos matemáticos e científicos.

   Exemplo (usando NumPy):
   ```python
   import numpy as np
   array = np.array([1, 2, 3, 4, 5])
   ```

Cada uma dessas estruturas de dados tem características distintas e é usada para resolver diferentes tipos de problemas em Python. A escolha da estrutura de dados depende das necessidades do seu programa ou projeto.

&nbsp;

<div align="center">
   
[Retornar ao índice](/README.md)

</div>