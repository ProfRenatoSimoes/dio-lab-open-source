# Modelo de Previsão de Vendas Mensais
[![NPM]([https://img.shields.io/npm/l/react)](https://github.com/ProfRenatoSimoes/dio-lab-open-source/new/main)
# Pontos de Extremidade:
# Endpoint 1: Dados Históricos de Vendas e Fatores Externos

Este ponto de extremidade recebe dados históricos de vendas mensais, bem como informações sobre fatores externos, como temperatura média, feriados, eventos, campanhas de marketing, etc.
Os dados históricos incluirão as vendas dos últimos 24 meses.

# Endpoint 2: Dados Atuais dos Fatores Externos

Este ponto de extremidade recebe dados em tempo real dos fatores externos relevantes, como a temperatura atual, eventos ocorrendo no mês atual, campanhas de marketing em curso, etc.
# Endpoint 3: Modelo de Previsão de Vendas

Este ponto de extremidade executa o modelo de previsão, utilizando os dados históricos e os dados atuais dos fatores externos para prever as vendas do próximo mês.
O modelo pode ser baseado em uma rede neural recorrente (RNN) para lidar com a natureza sequencial dos dados temporais e incorporar técnicas de atenção para ponderar a importância de diferentes fatores externos.
Fluxo de Funcionamento:
Os dados históricos e os dados atuais dos fatores externos são enviados aos seus respectivos pontos de extremidade.
O ponto de extremidade 3 recebe os dados do ponto de extremidade 1 e 2.
O modelo de previsão é alimentado com os dados fornecidos.
O modelo gera uma previsão para as vendas do próximo mês com uma margem de confiança.
A previsão é então enviada para um ponto de extremidade de saída.
Considerações Específicas do Modelo:
Rede Neural Recorrente (RNN):

Utilizada para capturar padrões temporais nos dados de vendas.
Pode ser uma LSTM (Long Short-Term Memory) ou GRU (Gated Recurrent Unit) para lidar com a longa dependência temporal.
Atenção Temporal:

Aplicada para ponderar a importância de diferentes pontos temporais nos dados históricos de vendas.
Isso permite que o modelo dê mais peso a períodos recentes que podem ser mais representativos das tendências atuais.
Atenção Contextual:

Aplicada para ponderar a importância dos diferentes fatores externos.
Por exemplo, se a temperatura atual estiver significativamente mais alta do que a média histórica para este período do ano, ela pode receber mais peso na previsão.e&logo=css3&logoColor=E94D5F)
![JavaScript](https://img.shields.io/badge/JavaScript-000?style=for-the-badge&logo=javascript&logoColor=30A3DC)
