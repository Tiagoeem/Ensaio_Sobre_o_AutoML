# Ensaio Sobre o AutoML

Este repositório será utilizado para análisar o desempenho das ferramentas de autoML [**PyCaret**](https://pycaret.org/) e [**H2O.ai**](https://www.h2o.ai/products/h2o-automl/). Ambas bibliotecas são open source e funcionam com diversas linguagens e plataformas.

## Metodologia

Ambas bibliotecas serão testadas quanto a sua capacidade de encontrar um bom modelo utilizando as configurações padrões das bibliotecas, customizando e uzando o pré processamento nas features dos datasets e em conjunto com uma modelagem apropriada do problema.

Serão utilizados dois datasets:
- ![#c5f015](https://via.placeholder.com/15/c5f015/000000?text=+) Fácil: Heart Disease da UCI - https://archive.ics.uci.edu/ml/datasets/Heart+Disease
  - Tipo: Classificação Binária
  - 13 features
  - 303 amostras
  - Sem missing
  - Sem necessidade de modelagem

- ![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+) Intermediário: Rain in Australia - https://www.kaggle.com/jsphyg/weather-dataset-rattle-package
  - Tipo: Classificação Binária
  - 22 features
  - 142193 amostras
  - Muitos missings
  - Existe necessidade de modelagem: Dados coletados em diversas cidades e com data que se repetem muitas vezes pelo dataset.

## Dados

Não é preciso baixar os dados, os notebooks possuem um link direto para o Google Colab em que o script pode ser executado diretamente. É utilizado a biblioteca gdown para baixar os dados automaticamente. **Então não se preocupe, de play e apenas relaxe**.

## Testes

Seguem a descrição de cada teste.

### Teste 1 - Default + Dataset Fácil ![#c5f015](https://via.placeholder.com/15/c5f015/000000?text=+) | [código-PyCaret](https://github.com/Tiagoeem/Ensaio_Sobre_o_AutoML/blob/main/Auto_ML_PyCaret_Heart.ipynb) | [H2O-em progresso](https://github.com/Tiagoeem/Ensaio_Sobre_o_AutoML)

Será utilizado o dataset Heart Disease, os dados não terão tratamento e os bibliotecas serão utlizadas com suas configurações "default".

### Teste 2 - Pre-Processamento + Customização de parâmetros + Dataset Fácil ![#c5f015](https://via.placeholder.com/15/c5f015/000000?text=+) | [código-PyCaret](https://github.com/Tiagoeem/Ensaio_Sobre_o_AutoML/blob/main/Auto_ML_PyCaret_Customizado_Heart.ipynb) | [H2O-em progresso](https://github.com/Tiagoeem/Ensaio_Sobre_o_AutoML)

Utilizando Heart Disease, os dados terão tratamento das próprias bibliotecas, além de "feature engeneering" e os bibliotecas serão utlizadas com suas configurações modificadas.

### Teste 3 - Default + Dataset Difícil ![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+)  | [código-PyCaret](https://github.com/Tiagoeem/Ensaio_Sobre_o_AutoML/blob/main/Auto_ML_PyCaret_Rain_Aus.ipynb) | [H2O-em progresso](https://github.com/Tiagoeem/Ensaio_Sobre_o_AutoML)

Será utilizado o dataset Rain in Australia, os dados não terão tratamento e os bibliotecas serão utlizadas com seus valores "default".

### Teste 4 - Pre-Processamento + Customização de parâmetros + Dataset Difícil ![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+) [em progresso](https://github.com/Tiagoeem/Ensaio_Sobre_o_AutoML)

Utilizando Rain in Australia, os dados terão tratamento das próprias bibliotecas, além de "feature engeneering" e os bibliotecas serão utlizadas com suas configurações modificadas.

### Teste 5 - Modelagem + Dataset Difícil ![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+) [em progresso](https://github.com/Tiagoeem/Ensaio_Sobre_o_AutoML)

Será realizado modelagem completa do problema antes de utilizar as bibliotecas.


## Resultados

### Resultado do teste 1

Dataset: Heart Disease ![#c5f015](https://via.placeholder.com/15/c5f015/000000?text=+)

**AutoML: PyCaret**
Melhor Classificador: Cat Boost

![resumo](https://raw.githubusercontent.com/Tiagoeem/Ensaio_Sobre_o_AutoML/main/suporte/imgs/pycaret/resumo_default_heart.png)

![auc](https://github.com/Tiagoeem/Ensaio_Sobre_o_AutoML/blob/main/suporte/imgs/pycaret/auc_default_heart.png?raw=true)
  
**AutoML: H2O.ai**

Em progresso.

### Resultado do teste 2

Dataset: Heart Disease ![#c5f015](https://via.placeholder.com/15/c5f015/000000?text=+)

**AutoML: PyCaret**
Melhor Classificador: Logistic Regression

![resumo](https://github.com/Tiagoeem/Ensaio_Sobre_o_AutoML/blob/main/suporte/imgs/pycaret/resumo_custom_heart.png?raw=true)

![auc](https://github.com/Tiagoeem/Ensaio_Sobre_o_AutoML/blob/main/suporte/imgs/pycaret/auc_custom_heart.png?raw=true)

### Resultado do teste 3

Dataset: Rain Australia ![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+)

**AutoML: PyCaret**
Melhor Classificador: LightGBM

![resumo](https://github.com/Tiagoeem/Ensaio_Sobre_o_AutoML/blob/main/suporte/imgs/pycaret/resumo_default_rain.png?raw=true)

![auc](https://github.com/Tiagoeem/Ensaio_Sobre_o_AutoML/blob/main/suporte/imgs/pycaret/auc_default_rain.png?raw=true)

### Resultado do teste 4

Dataset: Rain Australia ![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+)

Em progresso.

### Resultado do teste 5

Dataset: Rain Australia ![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+)

Em progresso.
