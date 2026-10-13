# Classificador supervisionado

Atividade de classificação de rostos usando a base **Labeled Faces in the Wild (LFW)**. O notebook explora os dados e compara KNN e SVM, com modelos baseline, redução de dimensionalidade por PCA e ajuste de hiperparâmetros. Também verifica a diferença entre o desempenho nos dados de treino e de teste.

## Como executar

1. Abra `template.ipynb` no Google Colab.
2. Envie `lfw-deepfunneled.zip` para a sessão do Colab, com o nome esperado pelo notebook.
3. Execute as células na ordem, de cima para baixo.

O notebook usa caminhos do Google Colab (`/content`). Para executá-lo em outro ambiente, os caminhos dos arquivos precisam estar disponíveis conforme indicado nas células.

## Verificações

As próprias células conferem a leitura das imagens, dimensões, valores de pixel, dados ausentes, divisão entre treino e teste e acurácia dos modelos. Ao final, compare as acurácias de treino e teste: uma diferença grande pode indicar overfitting; resultados baixos nos dois conjuntos podem indicar underfitting.

Após a leitura, espera-se encontrar 13.233 imagens e 5.749 classes. Para a classificação, o notebook mantém classes com pelo menos 20 imagens, resultando em 62 classes, e divide os dados em treino e teste. As métricas podem variar caso o ambiente, os dados ou os parâmetros sejam alterados.
