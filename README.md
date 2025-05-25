# Projeto IA - Classificação de Diagnóstico de Câncer de Mama

## Visão Geral
Este repositório contém o código e os arquivos auxiliares para o **Projeto-Desafio de Inteligência Artificial na Prática**, desenvolvido como parte de uma atividade acadêmica. O objetivo do projeto é criar um modelo de classificação binária para prever o diagnóstico de câncer de mama (maligno ou benigno) com base em 10 características de imagens de biópsia, utilizando o dataset **Breast Cancer Wisconsin (Diagnostic)** do UCI Machine Learning Repository.

O projeto foi dividido em dois níveis:
- **Nível I**: Análise exploratória, pré-processamento, treinamento e avaliação de modelos.
- **Nível II**: Avaliação adicional com 30 execuções, salvamento do modelo com `pickle`, e uma interface simples via linha de comando (CLI) para fazer predições.

## Dataset
- **Nome**: Breast Cancer Wisconsin (Diagnostic)
- **Link**: [UCI Repository](https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic)
- **Descrição**: O dataset contém 569 instâncias e 30 características numéricas derivadas de imagens de biópsias. Para este projeto, foram selecionadas as 10 primeiras características:
  - Raio médio
  - Textura média
  - Perímetro médio
  - Área média
  - Suavidade média
  - Compacidade média
  - Concavidade média
  - Pontos côncavos médios
  - Simetria média
  - Dimensão fractal média
- **Variável Alvo**: Diagnóstico (0 = Benigno, 1 = Maligno)

## Estrutura do Projeto
O projeto foi implementado em um notebook Jupyter e inclui os seguintes arquivos:
- **`ia_breast_cancer.ipynb`**: Notebook contendo o código completo do projeto, com comentários em português. Inclui:
  - Análise exploratória com gráficos (dispersão e distribuição).
  - Pré-processamento (padronização das variáveis).
  - Treinamento de dois modelos: Regressão Logística e Random Forest.
  - Avaliação dos modelos com acurácia.
  - Avaliação adicional com 30 execuções (Nível II).
  - Interface CLI para predição interativa.
- **`cancer_mama.pkl`**: Arquivo contendo o melhor modelo treinado (salvo com `pickle`).
- **`scaler_cancer_mama.pkl`**: Arquivo contendo o objeto `StandardScaler` treinado para padronizar os dados.

## Como Executar o Projeto
### Pré-requisitos
Para executar o projeto localmente, você precisará das seguintes ferramentas e bibliotecas:
- Python 3.8 ou superior
- Jupyter Notebook
- Bibliotecas Python:
  - `pandas`
  - `numpy`
  - `matplotlib`
  - `seaborn`
  - `scikit-learn`

Você pode instalar as dependências com o seguinte comando:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
