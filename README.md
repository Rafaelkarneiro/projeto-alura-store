# 📊 Análise de Desempenho das Lojas — Alura Store

## 📌 Descrição do Projeto

Este projeto faz parte de um **desafio de Análise de Dados com Python**, no qual o objetivo é auxiliar o **Senhor João**, proprietário da rede fictícia **Alura Store**, a decidir **qual loja deve ser vendida** para iniciar um novo empreendimento.

A decisão é baseada na análise de dados de vendas, categorias de produtos, avaliações de clientes e faturamento de **quatro lojas distintas**, utilizando técnicas de análise exploratória de dados (EDA) e visualização gráfica.

---

## 🎯 Objetivo

Identificar a loja com **menor eficiência geral**, considerando métricas relevantes como:

* Faturamento total das lojas  
* Quantidade de vendas por categoria de produto  
* Média de avaliação dos clientes  
* Comparação visual dos indicadores analisados  

Ao final, é apresentada uma **recomendação fundamentada em dados** sobre qual loja deve ser vendida.

---

## 🗂️ Fonte dos Dados

Os dados utilizados neste projeto são arquivos **CSV públicos**, disponibilizados pela Alura para fins educacionais, e são carregados diretamente de um repositório no GitHub.

As bases representam quatro lojas diferentes:

- `loja_1.csv`
- `loja_2.csv`
- `loja_3.csv`
- `loja_4.csv`

Os dados são importados diretamente via URL, conforme o trecho de código abaixo:

```python
import pandas as pd
import matplotlib.pyplot as plt

url = "https://raw.githubusercontent.com/alura-es-cursos/challenge1-data-science/refs/heads/main/base-de-dados-challenge-1/loja_1.csv"
url2 = "https://raw.githubusercontent.com/alura-es-cursos/challenge1-data-science/refs/heads/main/base-de-dados-challenge-1/loja_2.csv"
url3 = "https://raw.githubusercontent.com/alura-es-cursos/challenge1-data-science/refs/heads/main/base-de-dados-challenge-1/loja_3.csv"
url4 = "https://raw.githubusercontent.com/alura-es-cursos/challenge1-data-science/refs/heads/main/base-de-dados-challenge-1/loja_4.csv"

loja = pd.read_csv(url)
loja2 = pd.read_csv(url2)
loja3 = pd.read_csv(url3)
loja4 = pd.read_csv(url4)
```

Cada linha do dataset representa uma venda realizada, contendo informações como:

* Produto

* Categoria do produto

* Preço

* Frete

* Avaliação do cliente

* Localização geográfica

## **🛠️ Tecnologias Utilizadas**

* Python 3

* Pandas — manipulação e análise de dados

* Matplotlib — criação de visualizações

* Google Colab / Jupyter Notebook — ambiente de desenvolvimento

## **📊 Análises Realizadas**
###**💰 Faturamento Total das Lojas**

* Soma dos valores da coluna Preço para cada loja

* Identificação da loja com maior e menor faturamento

### **📦 Vendas por Categoria de Produto**

* Agrupamento dos dados pela coluna Categoria do Produto

* Contagem da quantidade de vendas por categoria

* Identificação das categorias mais populares

### **⭐ Média de Avaliação dos Clientes**

* Cálculo da média da coluna Avaliação da compra

* Comparação do nível de satisfação entre as lojas

## **📈 Visualizações Criadas**

Foram desenvolvidos **três tipos diferentes de gráficos**, conforme solicitado no desafio:

* **Gráfico de Barras**
→ Quantidade de vendas por categoria de produto

* **Gráfico de Linhas**
→ Média de avaliação dos clientes por loja

* **Gráfico de Dispersão**
→ Faturamento total das lojas

Essas visualizações auxiliam na interpretação dos dados e na identificação de padrões e diferenças entre as lojas.

## **🧠 Conclusão**

* A partir das análises realizadas, observou-se que:

* A Loja 1 apresenta o maior faturamento total

* A Loja 4 possui o menor desempenho financeiro

* As médias de avaliação dos clientes não variam proporcionalmente ao faturamento

* A distribuição das vendas por categoria não indica vantagem competitiva significativa da Loja 4

### **📌 Recomendação Final:**
Com base nos indicadores analisados, recomenda-se que o Senhor João venda a Loja 4, pois ela apresenta o menor faturamento e não se destaca positivamente nos demais critérios avaliados, tornando-se a opção mais estratégica para descontinuidade.

## **▶️ Como Executar o Projeto**

1. Clone o repositório:
```bash
git clone https://github.com/seu-usuario/seu-repositorio.git
```
2. Abra o notebook no Google Colab ou Jupyter Notebook

3. Execute as células sequencialmente para reproduzir as análises e gráficos

## **⚠️ Observações**

* Os dados utilizados são fictícios, destinados exclusivamente a fins educacionais

* O projeto foi desenvolvido com foco em clareza, organização e boas práticas

* O código pode ser facilmente adaptado para novos conjuntos de dados
