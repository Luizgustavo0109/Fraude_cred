# Fraude_cred


Este projeto consiste em um modelo de machine learn para lidar com um conjunto de dados desbalanceado de fraude de cartões de creditos. O dataset pode ser encontrado em <https://www.kaggle.com/datasets/isaikumar/creditcardfraud>.

O problema de classe desequilibrada é muito comum no modelo de classificação, onde a contagem de uma classe de variável de resposta é muito menor em comparação com outra classe. Como na detecção de fraude bancária, diagnóstico médico de doenças raras, etc., onde as contagens de fraude são muito menores em comparação com linhas sem fraude. Observou-se que os casos positivos de surdez ou fraude representam aproximadamente 2-3% do total de dados. Portanto, nesse cenário, às vezes, o algoritmo de aprendizado de máquina falha ao aprender o padrão subjacente e não consegue identificar corretamente os casos em que ocorre um padrão real.

Portanto, para lidar com esse tipo de problema é sobreamostrar a classe minoritária da variável de resposta e torná-la 50:50(class=0:class =1) ou 60:40(class=0:class =1).

>~~~python
> #Bibliotecas
> import pandas as pd
> import numpy as np
> import sklearn
> import seaborn

>**TÉCNICAS UTILIZADAS**
> * Regressão Logística
> * Random Forest
> * Minoritária de Oversampling
> * Função Resample do Sklearn
> * SMOTE

* **MÉTODOS UTILIZADOS PARA LIDAR COM O CONJUNTO DE DADOS DESBALANCEADOS**
1. UNDERSAMPLING MAJORITY CLASS/OVERSAMPLING

  >Subamostragem e sobreamostragem aleatórias. Um método amplamente adotado e talvez o mais direto para lidar com conjuntos de dados altamente desequilibrados é chamado de reamostragem. Consiste em remover amostras de classes majoritária (_subamostragem_) e/ou adicionar mais exemplos da classe minoritária (_sobreamostragem_).
  
2. SYNTHETIC MINORITY OVER-SAMPLING TECHNIQUE (SMOTE)

> É um algoritmo que pertence ao método de oversampling. O algoritmo _SMOTE_ funciona com base no princípio da sobreamostragem de amostras de dados minortários, gerando dados sintéticos. A sobreamostragem ocorre em relação a cada amostra minoritária.

