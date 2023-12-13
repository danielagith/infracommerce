# infracommerce
Processo Seletivo

Os notebooks deste projeto visam a construção de um modelo para fraude.
Para isto foram utilizados algoritmos de Árvore de Decisão, Florestas aleatórias e Redes Neurais afim de identificar qual teria a melhor resposta para este problema. 

Inclusive, há recomendação no site onde foi baixado o dataset para utilização de redes neurais para fazer o modelo.

Foi escolhido para esta análise o arquivo do site https://archive.ics.uci.edu/dataset/350/default+of+credit+card+clients, o terceiro da lista do repositório encaminhado. O mesmo não continha dados faltante.

No arquivo requirements_ tem as instalações que foram feitas no prompt para que o modelo pudesse ser construído e o dataset é o de no nome "defaultCreditcardClients.xls".

Para este processo seletivo, os arquivos que devem ser abertos são os notebooks infracommerce.ipynb e infracommerce_RedeNeural.ipynb. O primeiro notebook tem as predições feitas com Arvore de Decisão e Florestas Aleatórias e o segundo notebook o modelo foi gerado usando Rede Neural.

Para identificação dos melhores hiperparâmetros foi utilizada as bilbioteca GridSearchCV, RandomizedSearchCV que ajuda a identificar os hiperparêmetros que dão melhor resposta nos modelos tanto na Árvore de Decisão e Floresta Aleatória quanto no modelo com redes neurais.

Conclusão: Era esperado que o modelo usando redes neurais apresentasse uma melhor performance nas métricas em geral e que o modelo de florestas aleatórias também se comportasse melhor que o modelo utilizando árvore de decisão. Porém, embora os modelos tenham apresentado desempenhos muito próximos, para predição de fraude o modelo de floresta aleatória, neste estudo, se apresentou melhor nas métricas em relação aos demais modelos. Foi o que melhor respondeu na precisão pra fraude 73%, Recall 98% superior aos dos outros dois e com o mesmo F1-Score.

