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

## Leitura e reprodução

Os notebooks contêm código, etapas de modelagem e comentários sobre resultados anteriormente registrados. Nesta publicação, foram removidas as saídas de execução e adicionadas seções de análise crítica; os experimentos não foram reexecutados. Métricas históricas não representam validação independente.

Os notebooks originais usam caminhos do Google Drive. Para reexecutar os estudos no Colab, forneça as respectivas bases de dados, ajuste os caminhos locais e instale as dependências indicadas nos códigos. É importante revisar os procedimentos de imputação, reamostragem e seleção de variáveis para evitar vazamento de dados na avaliação preditiva.

As análises têm caráter educacional e experimental e não constituem instrumento de diagnóstico clínico ou tomada de decisão individual.

## Processamento de Linguagem Natural

O estudo de representação textual emprega um corpus de seis documentos, matrizes booleanas, TF, IDF, TF-IDF e índice invertido; explora modelos de embeddings Word2Vec, FastText, Wang2Vec e GloVe e discute Doc2Vec e Sentence-BERT. Os arquivos vetoriais pré-treinados e matrizes NumPy estão disponíveis na [pasta de origem no Drive](https://drive.google.com/drive/folders/1H2Vv6cJOLQtMhYvPaf7C8kCg_7kM38Kw), sem cópia para este repositório devido ao tamanho. O uso dos modelos requer configuração dos caminhos, dependências e verificação das respectivas condições de distribuição. As análises qualitativas de analogias não constituem avaliação estatística de superioridade entre arquiteturas.
