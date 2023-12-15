# infracommerce
Processo Seletivo

Os notebooks deste projeto visam a construção de um modelo para Inadimpência.
Para isto foram utilizados algoritmos de Árvore de Decisão, Florestas aleatórias e Redes Neurais afim de identificar qual teria a melhor resposta para este problema. 

Inclusive, há recomendação no site onde foi baixado o dataset para utilização de redes neurais para fazer o modelo.

Foi escolhido para esta análise o arquivo do site https://archive.ics.uci.edu/dataset/350/default+of+credit+card+clients, o terceiro da lista do repositório encaminhado. O mesmo não continha dados faltantes.

No arquivo requirements_ tem as instalações que foram feitas no prompt para que o modelo pudesse ser construído e o dataset é o de no nome "defaultCreditcardClients.xls".

Para este processo seletivo, os arquivos que devem ser abertos são os notebooks infracommerce.ipynb e infracommerce_RedeNeural.ipynb. O primeiro notebook tem as predições feitas com Arvore de Decisão e Florestas Aleatórias e o segundo notebook o modelo foi gerado usando Rede Neural.

Para identificação dos melhores hiperparâmetros foi utilizada as bilbioteca GridSearchCV, RandomizedSearchCV que ajuda a identificar os hiperparêmetros que dão melhor resposta nos modelos tanto na Árvore de Decisão e Floresta Aleatória quanto no modelo com redes neurais artificiais.

Conclusão: 

Era esperado que o modelo usando redes neurais apresentasse uma melhor performance nas métricas em geral, pois no site fonte do dataset também sugeria a utilização de redes neurais. E de fato foi o que ocorreu. Apesar de as métricas terem resultados muito próximos do modelo Random Forest

Foi o que melhor respondeu na precisão pra Inadimplência 71%, Recall 100% superior aos dos outros dois e com o mesmo F1-Score 88%.

Sobre a matriz de confusão: O algoritmo utilizando as redes neurais foi o que melhor trouxe também respostas para verdadeiros negativos e falsos negativos, o que traz melhor retorno financeiro e menos problemas de relacionamento com o cliente.

Porém, embora os modelos tenham apresentado desempenhos muito próximos, para predição de fraude o modelo de floresta aleatória, neste estudo, se apresentou melhor nas métricas em relação aos demais modelos. Foi o que melhor respondeu na precisão pra fraude 73%, Recall 98% superior aos dos outros dois e com o mesmo F1-Score 89%.

Sobre a matriz de confusão: O algoritmo de Florestas Aleatórias foi o que melhor trouxe também respostas para verdadeiros negativos e falsos negativos, o que traz melhor retorno financeiro e menos problemas de relacionamento com o cliente.


