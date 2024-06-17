## Como detectar Overfitting e Underfitting?

Primeiramente uma rápida revisão destes conceitos:

### Overfitting:

Quando o modelo não consegue generalizar para dados não vistos durante o treinamento, isso ocorre porque o modelo foi exposto a um conjunto de dados que não representa uma variação que existe no contexto de ambientes produtivos. O modelo pode apresentar bons resultados no treinamento, não porque conseguiu estabelecer uma fórmula matemática para o conjunto, mas porque memorizou características específicas dos dados de treinamento. 


### Underfitting:

Ocorre quando o modelo não é capaz de entender a fórmula para o conjunto de dados ainda na etapa de treinamento, o resultando em um desempenho insuficiente tanto nos dados de treinamento quanto nos dados de teste. 


### Como detectar esses problemas antes do ambiente produtivo?

Algumas instruções:

- Avaliar a diferença de desempenho entre o conjunto de treino e o conjunto de testes:
  
    -  Se o modelo apresentar um bom resultado no conjunto de treino e um mau resultado no conjunto de validação e/ou testes é um sinal clássico de overfitting.

- Se o modelo apresentar um mau resultado no conjunto de treino e de testes é um sinal de overfitting (este caso é menos comum).


#### Comparar os resultados com auxílio visual.

Se  plotarmos as predições dos conjuntos de treino e teste em um gráfico de linhas para efeitos comparativos, é possível identificar eventuais discrepâncias de maneira mais ágil. Uma grande diferença entre os resultados de ambos os conjuntos pode indicar overfitting.


#### Caso o modelo já esteja com overfitting, como tratar? 


- Colete mais dados para treino.
  
- Aplique [early stopping](https://github.com/octavioduarte/IA-AI/blob/master/04-estrategias-para-validacao-durante-o-treinamento-do-modelo/01-early-stopping.md) durante o treino.
  
- Reduza a complexidade das features (feature selection)

- Aplique data argumentation

- Utilize técnicas de regularização (L1, L2, dropout)
