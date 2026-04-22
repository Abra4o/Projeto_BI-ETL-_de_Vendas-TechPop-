# TechPop BI - ETL de Vendas 📊

** LINKEDIN: http://www.linkedin.com/in/abraão-luiz

Este projeto consiste em um pipeline de **Business Intelligence (BI)** que realiza o processo de **ETL (Extract, Transform, Load)** para converter dados de um sistema operacional (OLTP) em um Data Warehouse (OLAP). O objetivo é facilitar a análise estratégica de vendas, faturamento e desempenho de vendedores.

## 🚀 Objetivo do Projeto

Transformar os dados brutos do sistema operacional **FatorV** (PostgreSQL) em um modelo dimensional (**Star Schema**) hospedado na **Aiven Cloud**, permitindo visualizações claras sobre métricas de negócio como lucro total, faturamento por categoria e distribuição geográfica de fornecedores.

## 🛠️ Tecnologias Utilizadas

- **Linguagem:** Python 3.x
- **Manipulação de Dados:** Pandas
- **Conexão com Banco de Dados:** SQLAlchemy
- **Banco de Dados:** PostgreSQL (Hospedado na Aiven Cloud)
- **Visualização de Dados:** Matplotlib e Seaborn

## 📈 Arquitetura de Dados (Modelo Estrela)

O projeto transforma os dados originais nas seguintes tabelas dimensionais e de fato:

- **Dim_Cliente:** Informações cadastrais dos clientes.
- **Dim_Produto:** Detalhes dos produtos e suas categorias.
- **Dim_Vendedor:** Dados dos vendedores.
- **Dim_Fornecedor:** Localização e dados dos fornecedores.
- **Dim_Tempo:** Tabela de tempo gerada automaticamente para análises temporais.
- **Fato_Vendas:** Tabela central contendo métricas como valor total, lucro, quantidade vendida e comissões.

## 📋 Pré-requisitos

Antes de rodar o script, você precisará de:

1.  Uma conta na [Aiven Cloud](https://aiven.io/) (ou outro serviço PostgreSQL).
2.  Python instalado em sua máquina.
3.  Instalar as dependências do projeto:

```bash
pip install pandas sqlalchemy psycopg2-binary matplotlib seaborn python-dotenv
