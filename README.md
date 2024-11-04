# Atividade Prática - Redes Neurais para Diagnóstico de Diabetes

Este projeto implementa uma rede neural simples para prever a presença de diabetes em pacientes, usando o _dataset_ Pima Indians Diabetes Database. O objetivo é desenvolver um modelo de classificação binária que possa diferenciar entre pacientes com e sem diabetes com base em atributos de saúde.

## Estrutura do Projeto

### 1. Pré-processamento dos Dados

- Leitura do _dataset_ e separação das características e rótulos.
- Divisão em conjuntos de treino e teste.
- Padronização das variáveis de entrada para melhor desempenho do modelo.

### 2. Configuração do Modelo

- Modelo com três camadas ocultas e uma camada de saída para classificação binária.
- Funções de ativação: `Tanh` nas camadas ocultas e `Sigmoid` na saída.

### 3. Compilação e Treinamento

- Função de perda: `mean_absolute_error`.
- Otimizador: `RMSprop`.
- Métricas de avaliação: Acurácia, Precisão e Recall.
- Treinamento realizado com 1000 épocas e tamanho de lote de 64.

### 4. Avaliação do Modelo

- O modelo é avaliado em precisão e recall para determinar sua eficácia em prever corretamente a presença de diabetes.

### Ferramentas Utilizadas

- **Python** com **TensorFlow** e **Keras** para modelagem.
- **Scikit-Learn** para pré-processamento dos dados.
- **Pandas** para manipulação do _dataset_.

## Referência do Dataset

[Pima Indians Diabetes Database no Kaggle](https://www.kaggle.com/uciml/pima-indians-diabetes-database)
