# Predição Preços de Carros

## Descrição do Projeto
Objetico é realizar predições em um aplicativo de vendas de carros.
A qualidade e velocidade de predições é crucial para o negócio.
Acesso a dados históricos, especificações técnicas, versões de acabamento e preços.

## Ferramentas e Bibliotecas Utilizadas
- Python: Linguagem principal utilizada para a análise.
- Pandas e Numpy: Biblioteca para manipulação e análise de dados.
- Sklearn, lightgbm: Biblioteca para construção de modelo de machine learning.
- Matplotlib.pyplot e Seaborn: Biblioteca para construção de gráficos
- Time: Metrificar tempo de execução

## Tabela
O conjunto de dados possui os seguntes campos:
- DateCrawled — data em que o perfil foi baixado do banco de dados
- VehicleType — tipo de carroçaria do veículo
- RegistrationYear — ano de matrícula do veículo
- Gearbox — tipo de caixa de transmissão
- Power — potência (hp)
- Model — modelo do veículo
- Mileage — quilometragem (medida em km devido às especificidades regionais do conjunto de dados)
- RegistrationMonth — mês de registro do veículo
- FuelType — tipo de combustível
- Brand — marca do veículo
- NotRepaired — veículo reparado ou não
- DateCreated — data de criação do perfil
- NumberOfPictures — número de fotos do veículo
- PostalCode — código postal do proprietário do perfil (usuário)
- LastSeen — data da última atividade do usuário
- Price — preço (Euro)

## Metodologia
**Análise Exploratória de Dados**
- Importar as bibliotecas necessárias
- Carregar e visualizar os dados

**Pré-processamento**
- Dados ausentes
- Dados duplicados

**Preparação**
- Codificação de rótulos
- Seleção de features e target
- Divisão entre base de teste e treino

**Criação de Modelos**
- Calibração de hiperparâmetros
- Modelo LightGBM
- Modelo Floresta Aleatória
- Modelo Árvore de Decisão
- Modelo de Regressão Linear
- Análise das métricas dos modelos treinados

## Resultados
Para este projeto usamos os modelos de lightGBM, Floresta Aleatória, Árvore de Decisão e Regressão Linear para decidir qual o melhor modelo para nosso conjunto de dados. 
Testamos diferentes parâmetros no modelo lightGBM que variaram muito o tempo de execução do mesmo, por isso deixei o que está no projeto. 
Além de medir o tempo de execução de cada modelo avaliamos todos eles pelo REQM, e por isso, podemos escolher o modelo lightGBM como o melhor para essa tarefa, por mais que ele tenha o maior tempo de execução, é acetável.

## Aprendizados
- Análise de dados: interpretação e extração de insights valiosos a partir de grandes volumes de dados.
- Preparação do conjunto para aplicações em Machine Learning: separação do conjunto original em teste e treino, além da seleção das features e target do modelo.
- Regras de negócios: aplicação de regras de negócio para resolução de problemas.
- Aplicação de modelos de Machine Learning: aplicação, seleção de hiperparâmetros, teste e avalição do modelo.
- Documentação de projetos: elaboração de documentação clara e detalhada para garantir que o projeto seja compreensível e replicável.
- Utilização de bibliotecas e ferramentas: aplicação prática de diversas bibliotecas e ferramentas do ecossistema Python.
- Tomada de decisões baseadas em dados: uso de insights derivados da análise de dados para orientar decisões estratégicas.
