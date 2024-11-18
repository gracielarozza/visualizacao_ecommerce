# Projeto de Visualização de Dados de E-commerce

Este projeto é parte de um exercício do curso **Profissão Cientista de Dados** da Escola Britânica de Artes Criativas e Tecnologia (EBAC). No módulo 10, a tarefa era realizar uma análise visual dos dados fornecidos, criando os gráficos solicitados.

## Objetivo do Projeto  

O objetivo deste projeto é praticar a criação de gráficos a partir de um arquivo CSV. O processo inclui o pré-processamento dos dados antes da geração dos gráficos.

## Etapas do Projeto
### Importação e Análise Exploratória
   - Leitura dos dados de um arquivo CSV fornecido pelo professor.
   - Verificação da estrutura do DataFrame, valores nulos, duplicados e únicos.
   - Estatísticas descritivas iniciais.

### Tratamento de Dados
   - Preenchimento de valores nulos em colunas específicas.
   - Padronização de textos (letras minúsculas, remoção de caracteres especiais).
   - Correção e unificação de categorias inconsistentes (ex.: colunas `temporada`, `gênero`, `qtd_vendidos`).

### Codificação das Variáveis Categóricas
   - Codificação de variáveis categóricas utilizando `LabelEncoder`.

### Visualização dos Dados
   - **Mapa de calor:** correlação entre variáveis numéricas.
   - **Histogramas:** distribuições de `preço`, `nota` e `número de avaliações`.
   - **Gráficos de dispersão:** relação entre variáveis como `preço`, `número de avaliações` e `quantidade vendida`.
   - **Gráfico de densidade:** análise da densidade de `descontos`.
   - **Gráfico de barras:** `quantidade vendida` por `temporada`.
   - **Gráfico de pizza:** distribuição de produtos por `gênero`.

## Requisitos

- **Ambiente:** Jupyter Notebook ou Google Colab.
- **Python:** Versão 3.x ou superior.  
- **Dados:** Arquivo CSV `ecommerce_preparados.csv`.  
- **Bibliotecas necessárias:**
  - **Re**: Para operações com expressões regulares e manipulação de strings.  
  - **Pandas**: Para manipulação e limpeza dos dados.  
  - **Numpy**: Para operações numéricas e manipulação de arrays.  
  - **Matplotlib** e **Seaborn**: Para criação de gráficos.  
  - **Unidecode**: Para remover acentos e caracteres especiais das strings.  
  - **Scikit-learn**: Para codificação de variáveis categóricas, utilizando o `LabelEncoder`.

```python  
import re
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
from unidecode import unidecode
from sklearn.preprocessing import LabelEncoder
```
## Como Usar

1. Clone este repositório ou copie o código para o seu ambiente de trabalho.  
2. Instale as dependências necessárias.  
3. Caso necessário, substitua o caminho do arquivo CSV no código.  
4. Execute as células do notebook na ordem sequencial.  

## Licença

MIT