# 🚀 Desafio Técnico - Engenheiro de Dados Júnior (Gaudium)
# Autor: Gabriel da Silva Siqueira

## 🧾 Descrição
Este projeto tem como objetivo aplicar técnicas de modelagem dimensional a partir de uma tabela única de dados brutos contendo informações de vendas, produtos e clientes.  
A partir dessa base, foram criadas tabelas fato e dimensões utilizando PySpark e Spark SQL.

## 📁 Estrutura dos Dados

Arquivo de entrada: `dados_brutos.csv`  
Colunas disponíveis:
- nome_cliente
- cidade
- estado
- nome_produto
- categoria
- fabricante
- data
- qtd_vendida
- valor_total

## 🏗 Modelagem Criada

- **dim_cliente**  
  Contém informações únicas sobre os clientes.

- **dim_produto**  
  Contém informações únicas sobre os produtos vendidos.

- **dim_localidade**  
  Contém informações únicas de cidade e estado.

- **dim_tempo**  
  Derivada da coluna `data`, com ano, mês e dia.

- **fato_vendas**  
  Tabela principal contendo os fatos de vendas (com chaves para as dimensões).

## 🛠 Tecnologias Utilizadas

- PySpark
- Spark SQL
- Git e GitHub

## 📂 Arquivos no Repositório

- `casegaudium.ipynb` - Notebook com todo o código usado.
- `dim_cliente.csv`, `dim_produto.csv`, `dim_localidade.csv`, `dim_tempo.csv`, `fato_vendas.csv` - Tabelas exportadas.
- `README.md` - Este documento.

## ▶️ Como Executar

1. Certifique-se de ter um ambiente com suporte a PySpark (ex: Databricks, AWS EMR, máquina local com Spark instalado).
2. Suba o arquivo `dados_brutos.csv` e o notebook.
3. Execute o notebook `casegaudium.ipynb`.
4. As tabelas modeladas serão salvas na pasta `tabelas_fato_dim` em formato `.csv`.

## ✅ Observações

- A modelagem foi desenvolvida com base no esquema estrela.
- O foco principal foi demonstrar a criação e transformação dos dados de forma limpa, escalável e eficiente.