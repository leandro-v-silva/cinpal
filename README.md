graph TD
    %% Fact Table
    FactSales[Sales (Fact)]

    %% Dimension Tables
    DimDate[Date (Dimension)]
    DimCustomer[Customer (Dimension)]
    DimProduct[Product (Dimension)]
    DimStore[Store (Dimension)]

    %% Relationships
    FactSales -- OrderDate --> DimDate
    FactSales -- CustomerKey --> DimCustomer
    FactSales -- ProductKey --> DimProduct
    FactSales -- StoreKey --> DimStore
