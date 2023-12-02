# Detecção de Pulsares usando Machine Learning

## Introdução

Os pulsares são estrelas de nêutrons altamente magnetizadas que emitem feixes de radiação eletromagnética detectáveis à medida que giram. Este projeto utiliza técnicas de Machine Learning para identificar pulsares em um conjunto de dados estelar.

## Por que utilizar Machine Learning para identificar Pulsares?

A detecção manual de pulsares em grandes conjuntos de dados estelares pode ser desafiadora e demorada. A aplicação de algoritmos de Machine Learning oferece uma abordagem eficiente e automatizada para identificar padrões complexos que podem indicar a presença de pulsares.

## Modelos Supervisionados e Não Supervisionados

Ao abordar a detecção de pulsares, podemos explorar tanto modelos supervisionados quanto não supervisionados, dependendo da natureza dos dados.

A detecção de pulsares geralmente é uma tarefa de classificação binária, onde o objetivo é determinar se uma estrela é ou não um pulsar. Modelos não supervisionados podem ser mais adequados para tarefas de agrupamento, onde o objetivo é identificar padrões ou grupos naturais nos dados.

Por isso, optei por utilizar apenas algoritmos supervisionados.

### Modelos Supervisionados
Os modelos supervisionados são treinados em um conjunto de dados rotulado, onde as observações têm rótulos conhecidos. Neste projeto, três modelos supervisionados foram utilizados:

1. **Support Vector Classifier (SVC):** Este modelo busca encontrar um hiperplano que melhor separa as classes no espaço de características.
   
2. **KNeighborsClassifier:** KNeighborsClassifier classifica as observações com base nas classes de seus vizinhos mais próximos no espaço de características.

3. **Random Forest Tree:** Uma floresta aleatória é composta por várias árvores de decisão e produz uma classificação com base nas votações dessas árvores.

## Detecção de Pulsares usando Machine Learning

O dataset utilizado nesse projeto inclui as seguintes colunas:

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

A eficácia dos modelos é avaliada por meio de cinco métricas principais:

1. **Matriz de confusão (Confusion Matrix):** 

```math
\begin{matrix}TN&FP\\FN&TP\end{matrix}
```

- **TN (True Negative):** Observações corretamente classificadas como negativas.
- **FP (False Positive):** Observações incorretamente classificadas como positivas.
- **FN (False Negative):** Observações incorretamente classificadas como negativas.
- **TP (True Positive):** Observações corretamente classificadas como positivas.

2. **Acurácia:** 
   $$\ \text{Acurácia} = \frac{\text{Número de predições corretas}}{\text{Total de amostras}} \]$$

3. **F1-Score:** 
   $$\[ \text{F1-Score} = 2 \times \left( \frac{\text{Precisão} \times \text{Recall}}{\text{Precisão} + \text{Recall}} \right) \]$$

4. **Recall:** 
   $$\[ \text{Recall} = \frac{\text{Verdadeiros Positivos}}{\text{Verdadeiros Positivos + Falsos Negativos}} \]$$

5. **Precisão:** 
   $$\[ \text{Precisão} = \frac{\text{Verdadeiros Positivos}}{\text{Verdadeiros Positivos + Falsos Positivos}} \]$$


Quando lidamos com datasets desbalanceados, ou seja, quando a proporção entre as classes não é equitativa, a acurácia por si só, normalmente utilizada para avaliar um modelo, pode não ser uma métrica adequada. Isso ocorre porque um modelo pode alcançar uma alta acurácia simplesmente prevendo sempre a classe majoritária, ignorando completamente a classe minoritária.

Abaixo, segue uma descrição mais detalhada dos dois métodos de avaliação de desempenho dos modelos que devem ser priorizados, levando em consideração o contexto supracitado. 

1. **F1-Score:**
O F1-Score é a média harmônica entre precisão e recall. Ele é particularmente útil quando há um desequilíbrio entre as classes, pois leva em consideração tanto os falsos positivos quanto os falsos negativos.

2. **Matriz de Confusão:**
Analisar a matriz de confusão oferece insights sobre os erros específicos cometidos pelo modelo. Isso é crucial para entender como o modelo está lidando com a classe minoritária.

# Conclusão

Após a avaliação dos diferentes algoritmos de Machine Learning para a detecção de pulsares, observamos que todos os modelos apresentaram resultados similares e satisfatórios. A aplicação de técnicas de Machine Learning mostrou-se uma ferramenta promissora na área da astronomia, oferecendo uma abordagem eficiente para identificar pulsares em conjuntos de dados estelares complexos.

Esses resultados encorajam a continuação da exploração de técnicas de Machine Learning na astronomia.


