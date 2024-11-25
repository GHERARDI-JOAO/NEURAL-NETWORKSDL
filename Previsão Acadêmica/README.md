# Projeto de Classificação do Desempenho de Alunos

Este projeto foi desenvolvido como parte do curso _Redes Neurais e Deep Learning_, com o objetivo de aplicar técnicas de aprendizado profundo para resolver um problema de classificação. O dataset utilizado foi o **Student Performance Factors**, disponível na plataforma Kaggle, que fornece insights sobre diversos fatores que influenciam o desempenho acadêmico dos alunos.

---

## **Visão Geral do Dataset**

O dataset inclui 20 atributos relacionados ao desempenho acadêmico, tais como:

- **Horas de Estudo** (_Hours_Studied_): Número de horas dedicadas ao estudo por semana.
- **Frequência Escolar** (_Attendance_): Percentual de presença em aula.
- **Envolvimento dos Pais** (_Parental_Involvement_): Nível de participação dos pais na educação (Baixo, Médio, Alto).
- **Acesso a Recursos** (_Access_to_Resources_): Disponibilidade de recursos educacionais (Baixo, Médio, Alto).
- **Qualidade dos Professores** (_Teacher_Quality_): Avaliação da qualidade dos professores (Baixa, Média, Alta).
- **Pontuação no Exame** (_Exam_Score_): Nota final do exame (variável de saída).

O objetivo foi prever o desempenho dos alunos em três categorias:

- **Abaixo da média**
- **Média**
- **Acima da média**

---

## **Etapas do Desenvolvimento**

### 1. **Pré-processamento dos Dados**

- Conversão de variáveis categóricas, como _Parental_Involvement_, em valores numéricos com `LabelEncoder`.
- Normalização de dados numéricos, como _Hours_Studied_, utilizando `MinMaxScaler`.
- Categorização das notas (_Exam_Score_) em três classes com base em faixas de valores.

### 2. **Estrutura da Rede Neural**

- Rede composta por:
  - **3 camadas ocultas** com 128, 64 e 32 neurônios (ativação ReLU).
  - **Dropouts** para evitar overfitting.
  - **Camada de saída** com ativação softmax para classificação multiclasse.
- Otimizador **Adam** e função de perda `sparse_categorical_crossentropy`.

### 3. **Treinamento e Avaliação**

- Divisão dos dados em conjuntos de treino e teste (70%/30%).
- Validação cruzada durante o treinamento.
- Avaliação final:
  - **Acurácia**: 92,08%
  - **Loss**: 0,1860

---

## **Resultados Obtidos**

- O modelo obteve um desempenho robusto, classificando corretamente 1826 dos 1983 exemplos de teste.
- A alta acurácia demonstra a eficácia do modelo em prever o desempenho acadêmico com base nos fatores fornecidos.

---

## **Ferramentas Utilizadas**

- **Linguagem**: Python
- **Bibliotecas**:
  - Manipulação de Dados: NumPy, Pandas
  - Visualização: Matplotlib
  - Pré-processamento e Machine Learning: Scikit-learn
  - Deep Learning: TensorFlow/Keras

---

## **Conclusão**

Este projeto demonstrou como redes neurais podem ser aplicadas em problemas educacionais, oferecendo insights valiosos para professores e instituições. O modelo desenvolvido pode ser usado para identificar alunos que necessitam de suporte acadêmico e para criar estratégias de ensino personalizadas.

---

## **Como Executar**

1. Clone este repositório.
2. Instale as dependências listadas no arquivo `requirements.txt`.
3. Execute o código em um ambiente Jupyter Notebook ou diretamente em Python.
4. Certifique-se de configurar o caminho para o dataset ou importá-lo diretamente do Kaggle.

---

## **Referências**

- Dataset: [Student Performance Factors no Kaggle](https://www.kaggle.com/datasets/lainguyn123/student-performance-factors/data)
- [Professor: Denilson Alves Pereira - Universidade Federal de Lavras](https://sites.google.com/ufla.br/denilsonpereira/home?authuser=0)
