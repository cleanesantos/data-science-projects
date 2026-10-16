# Portfólio de Ciência de Dados

Coleção de projetos de Ciência de Dados, Estatística e Aprendizado de Máquina, organizados por método e aplicação. Os notebooks são estudos técnicos elaborados em Python e Google Colab.

## Projetos publicados

| Técnica | Estudo |
| --- | --- |
| Árvore de decisão | [Classificação de diabetes](machine-learning/decision-tree/diabetes_portfolio.ipynb) |
| Random Tree e Random Forest | [Comparação de modelos de classificação](machine-learning/random-forest/random-tree-random-forest.ipynb) |
| Redes neurais | [Classificação na base Adult Income](machine-learning/neural-networks/adult-income-neural-networks.ipynb) |
| K-means | [Análise de agrupamentos da base Adult Income](machine-learning/clustering-kmeans/adult-income-kmeans.ipynb) |
| PLN: representação textual | [Bag-of-Words, TF-IDF, índice invertido e embeddings](natural-language-processing/text-representations/atividade1-pln.ipynb) |
| PLN: versão comentada | [Notebook comentado de representação textual](natural-language-processing/text-representations/atividade1-pln-comentada.ipynb) |
| PLN aplicado: avaliações de consumidores | [Voz do consumidor: análises e classificação de reviews B2W](natural-language-processing/customer-reviews-b2w/analise_pln_b2w_voz_consumidor.ipynb) |

## Leitura e reprodução

Os notebooks contêm código, etapas de modelagem e comentários sobre resultados anteriormente registrados. Nesta publicação, foram removidas as saídas de execução e adicionadas seções de análise crítica; os experimentos não foram reexecutados. Métricas históricas não representam validação independente.

Os notebooks originais usam caminhos do Google Drive. Para reexecutar os estudos no Colab, forneça as respectivas bases de dados, ajuste os caminhos locais e instale as dependências indicadas nos códigos. É importante revisar os procedimentos de imputação, reamostragem e seleção de variáveis para evitar vazamento de dados na avaliação preditiva.

As análises têm caráter educacional e experimental e não constituem instrumento de diagnóstico clínico ou tomada de decisão individual.

## Processamento de Linguagem Natural

O estudo de representação textual emprega um corpus de seis documentos, matrizes booleanas, TF, IDF, TF-IDF e índice invertido; explora modelos de embeddings Word2Vec, FastText, Wang2Vec e GloVe e discute Doc2Vec e Sentence-BERT. Os arquivos vetoriais pré-treinados e matrizes NumPy estão disponíveis na [pasta de origem no Drive](https://drive.google.com/drive/folders/1H2Vv6cJOLQtMhYvPaf7C8kCg_7kM38Kw), sem cópia para este repositório devido ao tamanho. O uso dos modelos requer configuração dos caminhos, dependências e verificação das respectivas condições de distribuição. As análises qualitativas de analogias não constituem avaliação estatística de superioridade entre arquiteturas.

### Estudo aplicado: voz do consumidor

Análise independente do corpus B2W-Reviews01 com auditoria de qualidade, distribuição de notas, relação com recomendação, frequências lexicais, TF-IDF e classificação interpretável de textos da marca Samsung. O experimento foi executado com 132.373 avaliações na base total; no recorte modelado, 5.169 textos distintos, F1 macro de 0,8734 e AUC ROC de 0,9722 em um teste estratificado reservado (25%). Os valores **não** constituem validação externa. O notebook contém código para recalcular resultados ao receber o CSV original, disponível na [pasta de origem](https://drive.google.com/drive/folders/1VEffeCe6EGi0oVfsuPIkHrB5astVSv_K). O arquivo bruto não foi republicado por conter dados dos avaliadores.
