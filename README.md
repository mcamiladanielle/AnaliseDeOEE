## Analise de OEE
Conceito e Análise de OEE com Power BI

**1. Introdução**

O OEE (Overall Equipment Effectiveness), ou Eficiência Global do Equipamento, é um indicador amplamente utilizado na indústria para medir a produtividade de máquinas e processos.
De forma simples e direta, o OEE mostra quanto o equipamento foi efetivamente utilizado, relacionando a produção de itens bons com a capacidade total de produção.

A fórmula clássica é:
OEE = Disponibilidade * Desempenho * Qualidade

<img width="926" height="528" alt="OEEpg" src="https://github.com/user-attachments/assets/d3b168fd-b3a6-4e29-9005-1fc2ce9818b8" />

**2. Pilares do OEE**

🔹 **Disponibilidade**
Mede o tempo em que o equipamento esteve disponível para produção em relação ao tempo planejado

Impacto: Paradas não planejadas reduzem diretamente este índice.

🔹 **Desempenho**
Avalia a velocidade de produção em comparação ao tempo de ciclo esperado.

Impacto: Produção abaixo da capacidade teórica reduz o desempenho, já a produção acima da capacidade melhora o indicador,
mas gera o consumo de recursos não previstos e pode afetar outros processos/indicadores.

🔹 **Qualidade**
Mede a proporção de itens produzidos que atenderam às especificações (peças boas).

Impacto: Refugo e retrabalho reduzem o índice de qualidade.

🔹 **OEE Global**
Resultado da multiplicação dos três índices.
Permite identificar perdas e direcionar ações de melhoria de forma efetiva.

<img width="952" height="543" alt="Interferencias_oee" src="https://github.com/user-attachments/assets/ee7d6369-b118-4f11-882d-507a4ff2a73d" />

Fazendo uma analogia ao 5W1H, através do OEE, é  possível analisar O QUÊ (O impacto), QUAL (qual a voz de parada), QUANDO (data, turno) QUEM (o responsável) e ONDE (qual equipamento) ocorreram interferências que impactaram na eficiência global do equipamento, facilitando investigação das causas e a tomada de decisão para amenizar/eliminar o impacto negativo no principal indicador.
  
📊**3. Aplicação no Power BI**  

Utilizando o Power BI no processo de análise dos indicadores, é possivel obter insights no dia a dia da produção, em tempo real através de uma integração com MES/ERP.

-- Modelagem:
- Tratar tabelas de eventos de produção (tempo de máquina, paradas, peças boas/refugadas).
- Calcular métricas como Disponibilidade, Performance e Qualidade via DAX.

-- Dashboards:
- Visualizar OEE global e por máquina/grupo.
- Extratificar  perdas (setup, falhas, baixa velocidade, refugos).

**4. Tecnologias Utilizadas**

**Power BI** para construção dos dashboards.
**Power Query** para **ETL** e tratamento dos dados.
**Modelagem** de relacionamentos entre tabelas **fato** e **dimensão**.
Medidas **DAX** para cálculo dos índices de Disponibilidade, Desempenho, Qualidade e OEE.
**Storytelling** para apresentação clara e objetiva dos resultados.

Obs.: Os dados utilizados são fictícios, mas permitem aplicar as técnicas de análise do indicador OEE em ambiente de BI.

✅ **Benefícios**
- Possibilidade monitoramento em tempo real.
- Suporte à tomada de decisão para manutenção e operações em tempo real.
- Possibilidade de integração com MES/ERP para dados confiáveis.
  
Essas análises facilitam a investigação das causas e a tomada de decisão para reduzir ou eliminar impactos negativos na eficiência global da fábrica.
