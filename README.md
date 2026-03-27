# Análise de Vendas - Power BI

## Sobre o Projeto

Este projeto foi desenvolvido como parte de um case prático, com o objetivo de demonstrar habilidades em modelagem de dados, construção de dashboards e análise exploratória.

A base de dados contém informações de vendas, incluindo produtos, redes, lojas e localização geográfica (cidade e estado).

---

## Objetivo

Construir um dashboard interativo e intuitivo que permita:

* Analisar o desempenho de vendas por região
* Identificar os produtos mais relevantes (Curva de Pareto)
* Comparar a participação das redes ao longo do tempo
* Explorar dados por estado e cidade

---

## Modelagem de Dados

Foi aplicado o modelo **Star Schema (modelo estrela)** para garantir performance e escalabilidade.

### 🔹 Tabela Fato

* `Fato_Vendas`

  * Total de Vendas
  * Data
  * ProdutoID
  * RedeID
  * CidadeID
  * LojaID

### 🔹 Dimensões

* `Dim_Produto`
* `Dim_Rede`
* `Dim_Cidade`
* `Dim_Loja`
* `Dim_Data`

---

## Tratamento de Dados

Principais ajustes realizados no Power Query:

* Correção de inconsistências geográficas (cidade x estado)
* Padronização de textos (encoding de caracteres)
* Criação de chaves substitutas (IDs)
* Remoção de duplicidades
* Conversão de tipos de dados

---

## Principais Métricas (DAX)

Algumas medidas desenvolvidas:

* **Total de Vendas**
* **Quantidade de Cidades**
* **Vendas Média por Rede**
* **% de Vendas por Rede**
* **Crescimento Temporal**
* **Curva de Pareto (Ranking e % acumulado)**

---

## Dashboard

O dashboard foi estruturado para facilitar a leitura e geração de insights:

### 🔹 Visuais principais

* Mapa geográfico de vendas por região
* Curva de Pareto (produtos)
* Evolução temporal (% de vendas por rede)
* Top produtos mais vendidos
* Distribuição de vendas por rede
* KPIs principais (cards)

---

## Principais Insights

* As vendas estão concentradas nas regiões Sudeste e Sul
* Uma pequena quantidade de produtos representa a maior parte do faturamento (efeito Pareto)
* As redes apresentam variação de participação ao longo do tempo
* Algumas cidades se destacam como principais polos de venda

---

## Design e Usabilidade

* Interface limpa e intuitiva
* Uso de paleta de cores consistente
* Foco em clareza e leitura dos dados
* Filtros dinâmicos por UF e Cidade

---

## Tecnologias Utilizadas

* Power BI
* DAX
* Power Query (M)
* Modelagem de Dados

---

## 📌 Como Utilizar

1. Baixe o arquivo `.pbix`
2. Abra no Power BI Desktop
3. Interaja com os filtros (UF e Cidade)
4. Explore os visuais e insights

---

## 👨‍💻 Autor

Projeto desenvolvido por **Samuel Dias**
Analista de BI focado em dados, visualização e tomada de decisão orientada por dados.

---

## 📎 Observações

Este projeto foi desenvolvido para fins de avaliação técnica e portfólio, podendo conter simplificações em relação a cenários reais de produção.

---
