Dashboard de Previsão de Demanda de Café
📊 Sobre o Projeto

Este projeto tem como objetivo desenvolver uma solução analítica para previsão de demanda de café utilizando Power BI, permitindo o acompanhamento de indicadores estratégicos, análise histórica de consumo e suporte à tomada de decisão baseada em dados.

A solução foi construída seguindo as melhores práticas de Business Intelligence, contemplando desde a extração e transformação dos dados até a modelagem e criação de métricas avançadas para análise de desempenho.

🛠 Tecnologias Utilizadas
Microsoft Excel
Power BI Desktop
Power Query
Linguagem M
DAX (Data Analysis Expressions)
🔄 Processo ETL (Extract, Transform, Load)

O projeto utiliza uma base de dados em Excel como fonte principal de informações.

Durante a etapa de preparação dos dados foram aplicadas boas práticas de ETL utilizando o Power Query, incluindo:

Padronização de colunas
Tratamento de valores nulos
Correção de tipos de dados
Remoção de registros inconsistentes
Criação de colunas calculadas
Normalização de informações
Automatização das transformações através da Linguagem M
Exemplo de Recursos Utilizados na Linguagem M
Table.SelectRows()
Table.AddColumn()
Table.TransformColumnTypes()
Table.ReplaceValue()
Table.Group()
Funções customizadas para reaproveitamento de código
📐 Modelagem de Dados

A modelagem foi desenvolvida utilizando conceitos de:

Modelo Estrela (Star Schema)
Tabelas Fato e Dimensão
Relacionamentos otimizados
Redução de cardinalidade
Boas práticas de nomenclatura

Essa estrutura garante maior desempenho durante as consultas e cálculos analíticos.

⚡ Otimização e Performance DAX

As medidas DAX foram desenvolvidas seguindo técnicas de otimização para garantir melhor performance do modelo.

Principais Boas Práticas Aplicadas
Utilização de variáveis (VAR)
Reutilização de cálculos intermediários
Redução de context transitions desnecessárias
Simplificação de expressões complexas
Uso eficiente de CALCULATE()
Minimização de iterações em tabelas grandes
Exemplo
Receita Acumulada =
VAR ReceitaAtual =
    SUM(Vendas[Valor])

VAR ReceitaPeriodo =
    CALCULATE(
        ReceitaAtual,
        DATESYTD(Calendario[Data])
    )

RETURN
    ReceitaPeriodo

O uso de variáveis melhora a legibilidade do código, facilita a manutenção e reduz o processamento das medidas.

📈 Principais Indicadores

O dashboard disponibiliza análises relacionadas a:

Volume de vendas
Demanda projetada
Tendência de consumo
Receita
Ticket médio
Comparativos temporais
Evolução mensal
Indicadores de desempenho operacional
🎯 Objetivos do Projeto
Automatizar o processo de análise de demanda
Reduzir tempo gasto na consolidação de informações
Melhorar a qualidade dos dados
Apoiar decisões estratégicas
Aplicar boas práticas de ETL e modelagem analítica
Demonstrar conhecimentos avançados em Power BI, Power Query e DAX
🚀 Competências Demonstradas
Business Intelligence
Data Analytics
Data Modeling
ETL
Power Query
Linguagem M
DAX Avançado
Data Visualization
Performance Optimization
Dashboard Design
Forecasting e Análise Preditiva
