
# 📊 Previsão de Estoque Inteligente na AWS com [SageMaker Canvas](https://aws.amazon.com/pt/sagemaker/canvas/)

Desafio de projeto "Previsão de Estoque Inteligente na AWS com SageMaker Canvas". Neste Lab DIO, foi aprendido a usar o SageMaker Canvas para criar previsões de estoque baseadas em Machine Learning (ML). Abaixo estão os passos feitos para completar o desafio!

## 🚀 Passo a Passo

### 1. Selecionar Dataset

-   Navegue até a pasta `datasets` deste repositório. Esta pasta contém os datasets que você poderá escolher para treinar e testar seu modelo de ML. Sinta-se à vontade para gerar/enriquecer seus próprios datasets, quanto mais você se engajar, mais relevante esse projeto será em seu portfólio.
-   Escolha o dataset que você usará para treinar seu modelo de previsão de estoque.
-   Faça o upload do dataset no SageMaker Canvas.

### 2. Construir/Treinar

-   No SageMaker Canvas, importe o dataset que você selecionou.
-   Configure as variáveis de entrada e saída de acordo com os dados.
-   Inicie o treinamento do modelo. Isso pode levar algum tempo, dependendo do tamanho do dataset.

### 3. Analisar

-   Após o treinamento, examine as métricas de performance do modelo.
-   Verifique as principais características que influenciam as previsões.
-   Faça ajustes no modelo se necessário e re-treine até obter um desempenho satisfatório.

### 4. Prever

-   Use o modelo treinado para fazer previsões de estoque.
-   Exporte os resultados e analise as previsões geradas.
-   Documente suas conclusões e qualquer insight obtido a partir das previsões.

### 5. Resultado
-   Dataset utilizado: [Dataset](https://github.com/gabisoaress18/lab-aws-sagemaker-canvas-estoque/blob/0eff36dec724ca22e4088dc1480012556fd2112f/datasets/dataset-1000-com-preco-variavel-e-renovacao-estoque.csv)
-   Avg. wQL = 0.259, o que indica que o modelo é bem preciso.
-   MAPE = 1.803. O erro percentual médio absoluto (MAPE) é o erro percentual (diferença percentual entre o valor médio previsto e o valor real) calculado em média em todos os pontos de tempo. Um valor menor indica um modelo mais preciso com MAPE=0 como um modelo perfeito e sem erros. Como nesse modelo o MAPE foi de 1.803, podemos considerar que não é um modelo perfeito e apresenta erros.
-   WAPE = 0.378. O erro percentual absoluto ponderado (WAPE) mede o desvio geral dos valores previstos em relação aos valores observados e é definido pela soma do erro absoluto normalizado pela soma da meta absoluta. Um valor mais baixo indica um modelo mais preciso com WAPE=0 como um modelo perfeito e sem erros. Como nesse modelo o WAPE foi de 0.378, pode-er considerar que é como um modelo perfeito e sem erros.
-   RMSE = 29.146, indicando uma média quadrada dos erros quadrados médios alta, o que dá a entender que o modelo possui erros.
-   MASE = 1.393, indica o erro médio em escala absoluta, como nosso valor deu maior que 1, é um modelo estimado como pior que a linha de base.
