# Analisador de Vendas

Este projeto lê arquivos `.csv` contendo dados de vendas, realiza análises estatísticas básicas e gera gráficos para facilitar a visualização dos resultados. Foi desenvolvido com foco em praticar análise de dados com Python.

## Pré-requisitos

- Python 3.8 ou superior
- pandas
- matplotlib

## Instalação

Instale as bibliotecas necessárias usando o `pip`:

```bash
pip install pandas matplotlib
```

## Como usar

1. Clone o repositório:

```bash
git clone https://github.com/seuusuario/analisador-vendas.git
```

2. Execute o script principal:

```bash
python analisador.py
```

3. Siga as instruções para escolher o arquivo `.csv` a ser analisado.

Exemplo de uso básico no código:

```python
import pandas as pd
import matplotlib.pyplot as plt

dados = pd.read_csv('vendas.csv')
print(dados.describe())

dados['total_vendas'].plot(kind='bar')
plt.show()
```

## Exemplo de saída

> Estatísticas calculadas:

```
count    100.000000
mean     500.500000
std      288.819436
min      1.000000
25%      250.750000
50%      500.500000
75%      750.250000
max      1000.000000
```

## Exemplo de gráfico gerado

![Exemplo de Gráfico](grafico.svg)
