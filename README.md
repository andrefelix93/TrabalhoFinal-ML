# Transfer Learning com VGG16: Classificação de Flores usando Feature Extractor

Este projeto aplica a técnica de **Transfer Learning** usando o modelo **VGG16** para classificar imagens do **Flowers Dataset**. O objetivo é utilizar a abordagem de **Feature Extractor** para avaliar o desempenho do modelo sem a necessidade de treinar uma rede neural do zero.

## Tabela de Conteúdos
- [Introdução](#introdução)
- [Dataset](#dataset)
- [Técnica Utilizada](#técnica-utilizada)
- [Resultados](#resultados)
- [Nota Técnica](#nota-técnica)

---

## Introdução
O **Transfer Learning** é uma técnica poderosa que permite aproveitar modelos pré-treinados em grandes datasets (como a ImageNet) para resolver problemas específicos com datasets menores. Neste projeto, utilizamos o **VGG16**, um modelo clássico de deep learning, e o **Flowers Dataset**, que contém imagens de flores divididas em 5 classes.

A técnica de **Feature Extractor** consiste em congelar as camadas convolucionais do modelo pré-treinado e treinar apenas as camadas fully connected adicionadas no final. Isso é especialmente útil quando temos um dataset pequeno, pois evita o overfitting e reduz o tempo de treinamento.

---

## Dataset
O **Flowers Dataset** contém imagens de flores divididas em 5 classes:
- Daisy
- Dandelion
- Roses
- Sunflowers
- Tulips

O dataset foi dividido em conjuntos de **treino** e **validação**, com 80% das imagens usadas para treino e 20% para validação.

---

## Técnica Utilizada
- **Modelo**: VGG16.
- **Técnica**: Feature Extractor (congelamento das camadas convolucionais).
- **Data Augmentation**: Rotação, zoom, flip horizontal e outras transformações para aumentar a diversidade dos dados.
- **Métricas**: Acurácia e Loss.

---

## Resultados
O modelo alcançou os seguintes resultados:
- **Acurácia no Treino**: 87%
- **Acurácia na Validação**: 85%
- **Loss no Treino**: 25%
- **Loss na Validação**: 30%

---

### Pré-requisitos
- Python 3.x
- Bibliotecas: TensorFlow, Keras, NumPy, Matplotlib, scikit-learn

### Nota Técnica
Para mais detalhes sobre o projeto, confira a nota técnica no Medium:
https://medium.com/@dev.andresilva/transfer-learning-com-vgg16-classifica%C3%A7%C3%A3o-de-flores-usando-feature-extractor-151d9e294953

