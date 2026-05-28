# Dashboard de Vendas Olist - Base

<p align="left">
    <img src="https://raw.githubusercontent.com/Adriele-Cerqueira/Dashboard_Gerencial_OLIST/main/MENU.png" width="600">
  </p>

👉 [Abrir no Power Bi](https://app.powerbi.com/view?r=eyJrIjoiZGViYTRjZmMtYjNhNy00NWRkLTk3MDctODA3ZTE3NzAxZWUwIiwidCI6IjY1OWNlMmI4LTA3MTQtNDE5OC04YzM4LWRjOWI2MGFhYmI1NyJ9)

## Resumo Executivo

Este projeto em Power BI foi desenvolvido com base no dataset público de e-commerce da Olist, com foco na análise de vendas, desempenho comercial e comportamento operacional dos vendedores. Além da construção analítica tradicional, o projeto implementa uma solução personalizada de controle de acesso com Login, Senha e RLS dinâmica para múltiplos usuários utilizando o mesmo e-mail corporativo. O dashboard fornece uma visão executiva orientada à tomada de decisão, permitindo acompanhar faturamento, performance comercial, cancelamentos e evolução das vendas ao longo do tempo.

---

## Problema de Negócio

- Qual a tendência de crescimento das vendas ao longo do tempo em comparação ao ano anterior?
- Quais vendedores, estados e categorias de produtos possuem maior impacto no faturamento da operação?
- Qual o comportamento do ticket médio e da taxa de cancelamento durante o período analisado?
- Quais oportunidades de melhoria podem ser identificadas a partir da performance comercial e operacional dos vendedores?
- Qual a melhor forma de implementar controle de acesso individual dentro do Power BI em cenários onde múltiplos usuários compartilham o mesmo e-mail corporativo?

---

## Fonte de Dados

Os dados utilizados são provenientes do dataset público de e-commerce brasileiro disponibilizado pela Olist na plataforma Kaggle. O conjunto contém aproximadamente 100 mil pedidos realizados entre 2016 e 2018, abrangendo informações de clientes, vendedores, pagamentos, produtos, entregas e avaliações. Foram adicionadas tabelas complementares de Gerentes, Vendedores e Controle de Senhas para implementação da regra de acesso dinâmica.

Fonte oficial:  
[Kaggle - Brazilian E-commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

---

## Metodologia

- Tratamento e transformação de dados com Power Query (M)
- Modelagem dimensional e relacionamentos no Power BI
- Desenvolvimento de métricas e indicadores com DAX
- Criação de análises financeiras, operacionais e comparativas anuais
- Construção de KPIs como Ticket Médio e Taxa de Cancelamento
- Desenvolvimento de rankings e dashboards interativos
- Estruturação da navegação e experiência visual no Figma
- Implementação de autenticação personalizada com Login e Senha
- Aplicação de RLS dinâmica para controle de acesso por perfil e equipe

---

## Skills e Ferramentas

### Linguagens
- DAX
- Linguagem M

### Ferramentas de BI e Design
- Power BI
- Figma(prototipação de layouts e definição de interface/UI para experiência do usuário)

### Modelagem e Analytics
- Modelagem Dimensional
- Modelagem Estrela (Star Schema
- Data Visualization
- Storytelling com Dados
- Business Analytics
- KPI Design

---

## Indicadores-chave de desempenho (KPIs)

### 1. Faturamento Total
Mede o valor total vendido considerando preço dos produtos e valor de frete das transações realizadas.

### 2. Ticket Médio
Avalia o valor médio por pedido realizado, auxiliando na análise de rentabilidade comercial.

### 3. Total de Pedidos
Apresenta o volume total de pedidos processados no período analisado.

### 4. Taxa de Cancelamento
Monitora o percentual de pedidos cancelados em relação ao total de pedidos realizados.

### 5. Variação % vs Ano Anterior
Compara o desempenho do faturamento atual em relação ao ano anterior para análise de crescimento.

---

## Estrutura de Segurança e RLS Personalizada

Um dos principais diferenciais deste projeto foi a implementação de uma abordagem personalizada de controle de acesso dentro do Power BI.

Diferente da RLS tradicional baseada em e-mail corporativo único por usuário, o cenário simulado considera múltiplos usuários utilizando o mesmo e-mail empresarial. Para resolver essa limitação, foi criada uma solução utilizando:

- Tabela de Usuários
- Tabela de Senhas
- Relacionamento entre Gerentes e Vendedores
- Medidas DAX para autenticação
- Validação dinâmica de Login e Senha
- Restrição de visualização por equipe associada

Com isso, cada gerente consegue visualizar exclusivamente os vendedores sob sua responsabilidade, simulando um ambiente corporativo mais próximo de cenários reais de governança e segurança analítica.

---

## Insights das Páginas do Dashboard

### Visão Geral

A análise consolidada mostrou crescimento de aproximadamente 21% em relação ao ano anterior, com faturamento superior a R$ 864 milhões e baixa taxa de cancelamento. São Paulo concentrou o maior volume de vendas, enquanto categorias como Beleza & Saúde lideraram o faturamento.

<p align="left">
    <img src="https://raw.githubusercontent.com/Adriele-Cerqueira/Dashboard_Gerencial_OLIST/main/Geral.png" width="600">
  </p>

### Vendas

Os pagamentos via cartão de crédito representaram a maior parte do faturamento da operação. O estado de São Paulo apresentou maior concentração de pedidos e faturamento, enquanto regiões específicas demonstraram tickets médios mais elevados, indicando potencial de segmentação comercial.

<p align="left">
    <img src="https://raw.githubusercontent.com/Adriele-Cerqueira/Dashboard_Gerencial_OLIST/main/Vendas.png" width="600">
  </p>

### Equipe

A análise de performance dos vendedores revelou diferenças significativas entre faturamento, ticket médio e atingimento de metas. Alguns vendedores apresentaram alta receita com baixa eficiência de metas, enquanto outros superaram os objetivos definidos, indicando oportunidades de revisão estratégica de performance.

<p align="left">
    <img src="https://raw.githubusercontent.com/Adriele-Cerqueira/Dashboard_Gerencial_OLIST/main/Equipe.png" width="600">
  </p>

### Produtos

As categorias Beleza & Saúde, Relógios e Cama/Mesa/Banho lideraram as vendas, enquanto categorias com baixo faturamento demonstraram oportunidades para campanhas promocionais ou revisão de portfólio. O percentual de pedidos entregues acima de 97% também evidencia eficiência operacional da operação logística.

<p align="left">
    <img src="https://raw.githubusercontent.com/Adriele-Cerqueira/Dashboard_Gerencial_OLIST/main/Produtos.png" width="600">
  </p>

---

## Resultados e Recomendações de Negócio

O principal insight identificado foi a concentração significativa do faturamento em poucos estados, vendedores e categorias de produtos, evidenciando oportunidades de expansão comercial regional e otimização do mix de produtos. A análise temporal também demonstrou crescimento consistente das vendas em relação ao ano anterior.

A implementação do sistema de Login, Senha e RLS dinâmica trouxe um diferencial técnico importante ao projeto, simulando um cenário corporativo real de governança de dados e controle de acesso hierárquico.

Do ponto de vista estratégico, o dashboard permite:

- monitorar performance comercial em tempo real
- identificar vendedores com baixa performance
- analisar comportamento regional de vendas
- acompanhar eficiência operacional
- priorizar categorias mais rentáveis
- reduzir riscos de acesso indevido às informações

Como impacto potencial, a solução pode contribuir para aumento de eficiência comercial, melhoria na tomada de decisão gerencial e fortalecimento da segurança analítica dentro da organização.

---

## Próximos Passos

### 1. Implementação de Forecast de Vendas

Adicionar modelos preditivos para projeção de faturamento e sazonalidade comercial.

### 2. Integração com Banco de Dados em Tempo Real

Substituir arquivos estáticos por atualização automatizada via banco SQL ou API.

### 3. Expansão da Camada de Segurança

Implementar autenticação integrada com Active Directory e regras avançadas de governança de acesso.

---

Obs.: Este projeto foi desenvolvido em parceria com meu colega Lorenzo. Aproveite para acompanhar o trabalho dele no GitHub: https://github.com/LoRodrig/Dashboard_Gerencial_Olist
