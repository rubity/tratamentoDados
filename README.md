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

1. **Acurácia (Accuracy):** Proporção de predições corretas em relação ao total.
   ![Fórmula da Acurácia](https://latex.codecogs.com/svg.latex?%5Ctext%7BAccuracy%7D%20%3D%20%5Cfrac%7B%5Ctext%7BN%C3%BAmero%20de%20predi%C3%A7%C3%B5es%20corretas%7D%7D%7B%5Ctext%7BTotal%20de%20amostras%7D%7D)

2. **F1-Score:** Métrica que combina precisão e recall, útil quando as classes estão desbalanceadas.
   ![Fórmula do F1-Score](https://latex.codecogs.com/svg.latex?%5Ctext%7BF1-Score%7D%20%3D%202%20%5Ctimes%20%5Cleft%28%20%5Cfrac%7B%5Ctext%7BPrecis%C3%A3o%7D%20%5Ctimes%20%5Ctext%7BRecall%7D%7D%7B%5Ctext%7BPrecis%C3%A3o%7D%20%2B%20%5Ctext%7BRecall%7D%7D%20%5Cright%29)

3. **Recall (Sensibilidade):** Proporção de verdadeiros positivos em relação ao total de positivos reais.
   ![Fórmula do Recall](https://latex.codecogs.com/svg.latex?%5Ctext%7BRecall%7D%20%3D%20%5Cfrac%7B%5Ctext%7BVerdadeiros%20Positivos%7D%7D%7B%5Ctext%7BVerdadeiros%20Positivos%20&plus;%20Falsos%20Negativos%7D%7D)

4. **Precisão:** Proporção de verdadeiros positivos em relação ao total de positivos previstos.
   ![Fórmula da Precisão](https://latex.codecogs.com/svg.latex?%5Ctext%7BPrecis%C3%A3o%7D%20%3D%20%5Cfrac%7B%5Ctext%7BVerdadeiros%20Positivos%7D%7D%7B%5Ctext%7BVerdadeiros%20Positivos%20&plus;%20Falsos%20Positivos%7D%7D)

Certifique-se de ajustar os parâmetros dos algoritmos e explorar diferentes estratégias de pré-processamento para otimizar o desempenho do modelo na detecção de pulsares.


