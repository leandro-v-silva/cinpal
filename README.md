# Cinpal - Test (PBIP)

Este formato de projeto Power BI (PBIP) para integração com Git.

## Tecnologias Utilizadas

* **Power BI Desktop**
* **Formato PBIP**
* **Tabular Editor 2**
* **DAX**
* **Git**

## Modelagem de Dados (Star Schema)

O modelo de dados:

```mermaid
graph TD
    %% Tabela Fato
    FatoSales[Fato: sales]

    %% Tabelas Dimensão
    DimDate[Dim: Date]
    DimProduct[Dim: product]
    DimCustomer[Dim: customer]
    DimStore[Dim: store]

    %% Relacionamentos
    FatoSales -- OrderDate --> DimDate
    FatoSales -- ProductKey --> DimProduct
    FatoSales -- CustomerKey --> DimCustomer
    FatoSales -- StoreKey --> DimStore
