### Adicionando a etapa de validação

<i>Antes de continuarmos é importante destacar que o texto a seguir é para modelos mais complexos com um grande volume de dados.</i>


A validação durante o treinamento do modelo é essencial para identificar potenciais falhas antes dos testes finais. Por exemplo, ao dividir uma base de dados de 10 milhões de registros em conjuntos de treino e teste (como 90% e 10%, respectivamente), a validação permite monitorar o desempenho do modelo sem esperar pelo tempo e recursos computacionais exigidos pelos testes completos. Dessa forma, podemos ajustar o modelo gradualmente, reduzindo o tempo necessário para alcançar um resultado ideal.

Nestes casos **opte por extrair dados do conjunto de teste**, quanto mais dados dedicados o para o treino (tender a ser) melhor o resultado do modelo.

Então para concluir:

- Conjunto de testes: Utilizo depois do treinamento e validação do modelo.
- Conjunto de validação: Utilizo em paralelo ao treinamento.