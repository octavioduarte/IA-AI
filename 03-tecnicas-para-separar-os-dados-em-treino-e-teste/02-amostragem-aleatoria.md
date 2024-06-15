### Amostragem aleatória

Amostragem aleatória é uma estratégia na qual embaralhamos a ordem dos nossos dados para evitar viés no modelo.

Imagine que o modelo está percorrendo os dados de treino organizados da seguinte forma:

| feature1 | feature2 | class |
|----------|----------|-------|
| 3        | 6        | 1     |
| 5        | 15       | 1     |
| 7        | 13       | 1     |
| 9        | 31       | 1     |
| 1        | 29       | 1     |
| 3        | 18       | 1     |
| 1        | 4        | 1     |
| 2        | 10       | 0     |
| 4        | 12       | 0     |
| 6        | 14       | 0     |

Aqui estão os dados de treinamento em pequena escala. Observa-se que os 7 primeiros registros pertencem a uma única classe. Isso pode enviesar as previsões do modelo, levando-o a tender a classificar a maioria dos conjuntos como pertencentes à classe 1.

A ideia da amostragem aleatória é diversificar a amostragem de forma que o modelo não fique enviesado, algo como: 


| feature1 | feature2 | class |
|----------|----------|-------|
| 3        | 6        | 1     |
| 5        | 15       | 1     |
| 2        | 10       | 0     |
| 7        | 13       | 1     |
| 1        | 29       | 1     |
| 4        | 12       | 0     |
| 9        | 31       | 1     |
| 1        | 4        | 1     |
| 6        | 14       | 0     |


Treinar o modelo sem a diversificação na amostragem pode gerar resultados desastrosos, conforme o serviço de reconhecimento da Amazon que em 2020 deu respostas enviesadas para pessoas pretas 👇

https://exame.com/tecnologia/impreciso-com-negros-sistema-de-reconhecimento-facial-da-amazon-e-suspenso/