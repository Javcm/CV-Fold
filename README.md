# CV-Fold
Using CV-FOLD to get the best parameters to classificate tree diferent data sets:

- MNIST digits data set (60,000 digitalized hand written digits)
- Fruits data set (10 pictures of 13 different fruits)
- Embeddings from a bag of words model of 400 reviews on 8 categorías with 2 associated sentiments.

MNIST-digits data set with 5 classificators: -Support vectors machine -Logistic regression -Decision tree -Ada boost -MLP classifier  Obtaining the best score with support vector machine and Neural Networks.

Using the next parameters:

## Clasificadores de soporte vectorial (SVC)
    -Parámetro de regularización (C): {0.001, 0.01, 0.1, 1, 10, 100}
    -Kernel: {Lineal, Función de base radial (rbf)}
    -Coeficiente del Kernel ($\gamma$): { 0.001, 0.01, 0.1, 1, 10, 100 }

## Regresión Logística (Reg Logit)
    - Parámetro de regularización (C): {0.1, 1, 10, 100}
    - Algoritmo de optimización: {Limited Memory Broyden–Fletcher–Goldfarb–Shanno , Gradiente Conjugado de Newton, SAGA}

## Árboles de decisión
    -Profundidad máxima:  [1,20]
    -Muestras mínimas para dividir: {2, 3, 4}
    -Criterio discriminativo: {Entropía, Ganancia de Información (Gini)}

## Ada Boost
Se utilizó Ada Boost sobre un modelo de árboles de decisión, usando como parámetros los valores óptimos encontrados en el árbol de decisión 
    -Número de estimadores: { 50, 100 }

## Perceptrón multicapa (MLP)
    Máximo de iteraciones: [100,200]
    Parámetro de regularización: {10^{-1}, 10^{-2}, 10^{-3}, 10^{-4}, 10^{-5}}
    Tamaño de capas escondidas: [10,15]
    
