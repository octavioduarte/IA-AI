### Model Checkpointing

Imagine o seguinte cenário: 

Você configurou seu modelo para usar a técnica de early stopping após 10 épocas, o que significa que se não houver melhoria a cada 10 iterações no conjunto de treinamento, o treinamento é interrompido. Por exemplo, na época 45, o treinamento foi interrompido porque não houve progresso desde a época 35. No entanto, até a época 34, o modelo mostrou evolução e identificou um conjunto de hiperparâmetros que melhoraram sua eficiência. Sem aplicar o `model checkpointing` este progresso significativo é perdido, por tanto em resumo aplicar esta técnica lhe garante que eventuais progressos durante o treinamento serão armazenadas em disco.