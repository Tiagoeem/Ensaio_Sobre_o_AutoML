# Ensaio Sobre o AutoML

Este repositório será utilizado para análisar o desempenho das ferramentas de autoML [**PyCaret**](https://pycaret.org/) e [**H2O.ai**](https://www.h2o.ai/products/h2o-automl/). Ambas bibliotecas são open source e funcionam com diversas linguagens e plataformas.

## Metodologia

Ambas bibliotecas serão testadas quanto a sua capacidade de encontrar um bom modelo utilizando as configurações padrões das bibliotecas, customizando e uzando o pré processamento nas features dos datasets e em conjunto com uma modelagem apropriada do problema.

Serão utilizados dois datasets:
- Fácil: Heart Disease da UCI: https://archive.ics.uci.edu/ml/datasets/Heart+Disease
  - Tipo: Classificação Binária
  - 13 features
  - 303 amostras
  - Sem missing
  - Sem necessidade de modelagem

- Intermediario: Rain in Australia: https://www.kaggle.com/jsphyg/weather-dataset-rattle-package
  - Tipo: Classificação Binária
  - 22 features
  - 142193 amostras
  - Muitos missings
  - Existe necessidade de modelagem: Dados coletados em diversas cidades e com data que se repetem muitas vezes pelo dataset.

## Dados

Não é preciso baixar os dados, os notebooks possuem um link direto para o Google Colab em que o script pode ser executado diretamente. É utilizado a biblioteca gdown para baixar os dados automaticamente. **Então não se preocupe, de play e apenas relaxe**.

## Testes

Seguem a descrição de cada teste.

### Teste 1 - Default + Dataset Fácil [notebook]()

Será utilizado o dataset Heart Disease, os dados não terão tratamento e os bibliotecas serão utlizadas com suas configurações "default".

### Teste 2 - Pre-Processamento + Customização de parâmetros + Dataset Fácil [em progresso](https://github.com/Tiagoeem/Ensaio_Sobre_o_AutoML)

Utilizando Heart Disease, os dados terão tratamento das próprias bibliotecas, além de "feature engeneering" e os bibliotecas serão utlizadas com suas configurações modificadas.

### Teste 3 - Default + Dataset Difícil [em progresso](https://github.com/Tiagoeem/Ensaio_Sobre_o_AutoML)

Será utilizado o dataset Rain in Australia, os dados não terão tratamento e os bibliotecas serão utlizadas com seus valores "default".

### Teste 4 - Pre-Processamento + Customização de parâmetros + Dataset Difícil [em progresso](https://github.com/Tiagoeem/Ensaio_Sobre_o_AutoML)

Utilizando Rain in Australia, os dados terão tratamento das próprias bibliotecas, além de "feature engeneering" e os bibliotecas serão utlizadas com suas configurações modificadas.

### Teste 5 - Modelagem + Dataset Difícil [em progresso](https://github.com/Tiagoeem/Ensaio_Sobre_o_AutoML)

Será realizado modelagem completa do problema antes de utilizar as bibliotecas.


## Resultados

### Resultado do teste 1

**AutoML: PyCaret**
Melhor Classificador: Cat Boost

<imagems>
  
**AutoML: H2O.ai**
Melhor Classificador: ?

<imagems>
  

### Resultado do teste 2

Em progresso.

### Resultado do teste 3

Em progresso.

### Resultado do teste 4

Em progresso.

### Resultado do teste 5

Em progresso.