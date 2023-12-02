# Detecção de Pulsares usando Machine Learning

## Introdução

Os pulsares são estrelas de nêutrons altamente magnetizadas que emitem feixes de radiação eletromagnética detectáveis à medida que giram. Este projeto utiliza técnicas de Machine Learning para identificar pulsares em um conjunto de dados estelar.

## Por que utilizar Machine Learning para identificar Pulsares?

A detecção manual de pulsares em grandes conjuntos de dados estelares pode ser desafiadora e demorada. A aplicação de algoritmos de Machine Learning oferece uma abordagem eficiente e automatizada para identificar padrões complexos que podem indicar a presença de pulsares.

## Detecção de Pulsares usando Machine Learning

Este projeto colaborativo implementa três algoritmos de Machine Learning para a detecção de pulsares: Support Vector Classifier (SVC), K-Nearest Neighbors (KNN) e Random Forest Tree. Esses algoritmos são treinados em um dataset que inclui as seguintes colunas:

1. **Mean of the integrated profile**: Média do perfil integrado.
2. **Standard deviation of the integrated profile**: Desvio padrão do perfil integrado.
3. **Excess kurtosis of the integrated profile**: Curtose em excesso do perfil integrado.
4. **Skewness of the integrated profile**: Assimetria do perfil integrado.
5. **Mean of the DM-SNR curve**: Média da curva DM-SNR.
6. **Standard deviation of the DM-SNR curve**: Desvio padrão da curva DM-SNR.
7. **Excess kurtosis of the DM-SNR curve**: Curtose em excesso da curva DM-SNR.
8. **Skewness of the DM-SNR curve**: Assimetria da curva DM-SNR.
9. **target_class**: Classe-alvo indicando se a estrela é ou não um pulsar.

## Avaliação do Modelo

A eficácia dos modelos é avaliada por meio de quatro métricas principais:

1. **Acurácia (Accuracy):** 
   \[ \text{Accuracy} = \frac{\text{Número de predições corretas}}{\text{Total de amostras}} \]

2. **F1-Score:** 
   \[ \text{F1-Score} = 2 \times \left( \frac{\text{Precisão} \times \text{Recall}}{\text{Precisão} + \text{Recall}} \right) \]

3. **Recall (Sensibilidade):** 
   \[ \text{Recall} = \frac{\text{Verdadeiros Positivos}}{\text{Verdadeiros Positivos + Falsos Negativos}} \]

4. **Precisão:** 
   \[ \text{Precisão} = \frac{\text{Verdadeiros Positivos}}{\text{Verdadeiros Positivos + Falsos Positivos}} \]


Certifique-se de ajustar os parâmetros dos algoritmos e explorar diferentes estratégias de pré-processamento para otimizar o desempenho do modelo na detecção de pulsares.


