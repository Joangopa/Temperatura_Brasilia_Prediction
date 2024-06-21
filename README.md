## 📊📈 Análise de Séries Temporais sobre o Clima em Brasília

 Durante este estudo, analisei uma série temporal de dados climáticos de Brasília, abrangendo os últimos 5 anos.

 ![imagem](https://github.com/Joangopa/predicao_temp_Sequencial/blob/main/imagens/serie.png)

 ### 🔍 Objetivo: 
 Utilizar um modelo sequencial com Keras para prever padrões climáticos futuros com base em dados históricos.

### 🔧 Abordagem Técnica:
- Dados: Utilizei um conjunto de dados climáticos fornecido pelo Instituto Nacional de Meteorologia (INMET), incluindo variáveis como temperatura, precipitação, umidade, entre outras, coletadas diariamente em Brasília nos últimos cinco anos.

- Modelo: Implementei um modelo Sequential() do Keras, uma ferramenta poderosa para construir redes neurais profundas. Essa escolha permite capturar as complexidades temporais nos dados climáticos e gerar previsões precisas.

### Características Principais:
- Pré-processamento: Normalização dos dados e criação de características temporais para enriquecer o modelo.
- Camadas:
- - LSTM: Utilizei uma camada LSTM com 64 unidades para capturar padrões temporais.
- - Dense: Adicionei uma camada densa com 8 unidades e função de ativação ReLU, seguida de uma camada de saída com função de ativação linear para prever valores contínuos.
- Compilação: O modelo foi compilado com a função de perda Mean Squared Error e o otimizador Adam com uma taxa de aprendizado de 0.0001.
- Treinamento: Treinei o modelo por 10 épocas com validação cruzada, utilizando ModelCheckpoint para salvar o melhor modelo baseado na métrica de Root Mean Squared Error.

 ![imagem](https://github.com/Joangopa/predicao_temp_Sequencial/blob/main/imagens/test.png)
