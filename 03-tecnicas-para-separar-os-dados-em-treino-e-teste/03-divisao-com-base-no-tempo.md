### Divisão dos dados com base no tempo

Em cenários onde o tempo é uma feature do modelo, é uma prática recomendada separar os dados de forma ascendente. Por exemplo, se os dados estão distribuídos ao longo de 12 meses, podemos usar os dados de Janeiro a Agosto para treinamento e os dados de Setembro a Dezembro para validação.

Nesse contexto, não é aconselhável usar amostragem aleatória, pois a ordem cronológica dos dados possui um peso significativo na predição do modelo. Separar os dados de forma ascendente, por exemplo, utilizando os dados de Janeiro a Agosto para treinamento e de Setembro a Dezembro para validação, ajuda o modelo a aprender sequências temporais corretas e a evitar viéses que poderiam influenciar negativamente suas previsões.
