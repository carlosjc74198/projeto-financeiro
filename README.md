# Sistema de Análise Financeira

## 📊 Sobre o Projeto

Este é um sistema de análise financeira que gerencia e analisa dados de vendas, produtos e descontos. O projeto utiliza uma estrutura de banco de dados relacional para armazenar e processar informações sobre transações comerciais, produtos e métricas de desempenho.

## 🏗️ Estrutura do Banco de Dados

Tabelas Dimensões
D_Produtos
Armazena informações principais sobre os produtos e suas métricas de vendas.

ID_produto (Chave Primária)
Produto
Média de Unidades Vendidas
Médias do valor de vendas
Mediana do valor de vendas
Valor máximo de Venda
Valor mínimo de Venda

D_Produtos_Detalhes
Contém detalhes específicos sobre cada produto e suas características de venda.

ID_produtos (Chave Estrangeira)
Discount Band
Sale Price
Units Sold
Manufactoring Price

D_Descontos
Gerencia as informações sobre descontos aplicados aos produtos.

ID_produto (Chave Estrangeira)
Discount
Discount Band

D_Detalhes
Tabela com informações complementares (*)
D_Calendário
Dimensão de tempo gerada através de DAX utilizando a função calendar()
Tabela Fato
F_Vendas
Tabela principal que registra todas as transações de vendas.

SK_ID (Chave Surrogate)
ID_Produto
Produto
Units Sold
Sales Price
Discount Band
Segment
Country
Salers
Profit
Date

## 🔧 Tecnologias Utilizadas

SQL Server (ou especifique o banco de dados utilizado)
DAX (Data Analysis Expressions)
Power BI (se aplicável)

## 📈 Funcionalidades Principais

Análise detalhada de vendas por produto
Acompanhamento de descontos e margens de lucro
Análise geográfica de vendas por país
Monitoramento de performance de vendedores
Análise temporal de vendas

## 🚀 Como Utilizar

Clone o repositório
Configure o banco de dados seguindo o script de criação das tabelas
Importe os dados iniciais (se disponíveis)
Configure as conexões com suas ferramentas de análise

## 📝 Notas Adicionais

A tabela D_Calendário é gerada automaticamente utilizando DAX
Todas as análises de vendas consideram descontos e preços de manufatura
O sistema permite análises segmentadas por região e categoria de produto

## ✨ Atualizações Futuras Planejadas

Implementação de novos indicadores de performance
Integração com sistemas externos
Desenvolvimento de dashboards automatizados
