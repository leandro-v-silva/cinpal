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
gantt
    title Project Implementation Timeline
    dateFormat  YYYY-MM-DD
    axisFormat  %m-%d
    
    section Planning Phase
    Requirements Gathering   :active, req1, 2026-06-15, 5d
    Architecture Design      : des1, after req1, 7d
    
    section Development Phase
    Core Backend Dev         : dev1, after des1, 10d
    Frontend Integration     : dev2, after dev1, 8d
    
    section Testing & Deploy
    QA & Bug Fixing          : qa1, after dev2, 5d
    Production Release       : milestone, after qa1, 0d
