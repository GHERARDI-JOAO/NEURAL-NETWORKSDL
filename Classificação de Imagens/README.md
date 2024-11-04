# Atividade Prática - Redes Neurais para Classificação de Imagens

Este projeto implementa uma rede neural para classificar imagens de gatos e cachorros, utilizando o dataset disponível no Kaggle. O objetivo é desenvolver um modelo de classificação binária que possa diferenciar entre imagens de gatos e cães com base nas características visuais.

## Estrutura do Projeto

1. **Pré-processamento dos Dados**

   - Leitura do dataset e conversão das imagens em vetores de pixels.
   - Separação das imagens em conjuntos de treinamento (8.000 imagens) e teste (4.000 imagens).
   - Aumento de dados (data augmentation) para expandir o conjunto de treinamento e melhorar a robustez do modelo.

2. **Configuração do Modelo**

   - Modelo com camadas ocultas e uma camada de saída para classificação binária.
   - Funções de ativação: ReLU nas camadas ocultas e Softmax na camada de saída.

3. **Compilação e Treinamento**

   - Função de perda: categorical_crossentropy.
   - Otimizador: Adam.
   - Métricas de avaliação: Acurácia.
   - Treinamento realizado com um número definido de épocas e tamanho de lote.

4. **Avaliação do Modelo**
   - O modelo é avaliado com base na precisão em classificar corretamente as imagens de gatos e cachorros.

## Ferramentas Utilizadas

- Python com TensorFlow e Keras para modelagem.
- Keras Preprocessing para manipulação das imagens.
- Pandas para organização dos dados.

## Referência do Dataset

Dataset de imagens de gatos e cachorros disponível no Kaggle: [Kaggle Cats and Dogs Dataset](https://www.kaggle.com/datasets/d4rklucif3r/cat-and-dogs).

---
