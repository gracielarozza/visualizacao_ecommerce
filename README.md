# Visualização de Dados de E-commerce

## Objetivo

Este projeto tem como objetivo utilizar as bibliotecas **Matplotlib** e **Seaborn** para criar visualizações de dados relacionados às vendas de um E-commerce.

## Dados Utilizados

Após a importação do dataset, as seguintes colunas foram selecionadas, de acordo com a relevância para a análise gráfica e facilidade no tratamento:

```python
df = df[['Nota', 'N_Avaliações', 'Desconto', 'Gênero',
         'Temporada', 'Qtd_Vendidos', 'Preço']]
```
### Dicionário de Variáveis

- **Nota**: Avaliação recebida pelo produto, de 0 a 5.
- **N_Avaliações**: Quantidade total de avaliações registradas para o produto.
- **Desconto**: Percentual de desconto aplicado sobre o preço do produto.
- **Gênero**: Categoria de gênero atribuída ao produto.
- **Temporada**: Estação ou período de lançamento do produto.
- **Qtd_Vendidos**: Quantidade de unidades vendidas do produto.
- **Preço**: Valor de venda do produto.

## Tratamento de Dados

Durante o pré-processamento, foram realizadas as seguintes ações:

- **Tratamento de valores nulos** presentes em algumas colunas;
- **Padronização de formatos de texto**.
- **Remoção de inconsistências** em colunas categóricas como `Gênero` e `Temporada`, com padronização na escrita e substituição por categorias agrupadas.
- **Conversão de dados de vendas** para valores numéricos, substituindo expressões como '+10mil' por '10000';

Possíveis outliers foram observados em algumas variáveis. Mas, **não foram removidos**, pois nesse projeto o foco é a visualização.

## Principais insights

- Foram identificadas inconsistências no cadastro dos produtos, com muitas categorias que poderiam ser agrupadas e padronizadas para simplificar a catalogação.
- A maior parte dos produtos está concentrada em faixas de preço mais baixas, com pouco ou nenhum desconto.
- Há predominância de produtos voltados para o público feminino.
- A maioria dos produtos possui boa avaliação. Porém, também há casos de produtos bem avaliados com poucas vendas, o que pode indicar problemas de divulgação ou preço.
- Foi observada uma forte correlação entre o número de avaliações e a quantidade de vendas, o que reforça a influência das avaliações na decisão de compra.

## Bibliotecas Utilizadas

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`

## Arquivos

- `visualizacao_ecommerce.ipynb` - Notebook principal do projeto, que contém todo o tratamento de dados e visualizações.

## Observações

Este projeto foi desenvolvido com foco didático e tem como principal objetivo a prática de técnicas de visualização. Por isso, decisões de limpeza e análise foram feitas de forma simples, priorizando o aprendizado.

## Autoria

**Graciela Rozza** - Projeto desenvolvido como parte dos estudos em **Ciência de Dados**, com foco em **visualização e exploração de dados com Python**.

## Licença

MIT