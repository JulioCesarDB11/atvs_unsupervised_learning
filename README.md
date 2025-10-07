# 📊 Atividades de Clusterização (Aprendizado Não Supervisionado de Máquina)

Este repositório contém as implementações e análises dos principais algoritmos de clusterização, desenvolvidas como parte das atividades da disciplina de **Aprendizado Não Supervisionado de Máquina**.

Os notebooks exploram a teoria, a implementação do zero (com NumPy) e a aplicação prática de cada algoritmo em datasets clássicos (como Iris e Wine) e em problemas reais (como compressão de imagem e detecção de anomalias).

## 🗂️ Estrutura do Repositório

| Arquivo/Pasta | Algoritmo | Descrição |
| :--- | :--- | :--- |
| `02 - K-Means.ipynb` | **K-Means** | Implementação do algoritmo *K-Means* do zero. Inclui a fundamentação matemática, o **Método do Cotovelo** para determinação do $K$ ótimo e aplicações em compressão/segmentação de imagens. |
| `03 - Hierarchical.ipynb` | **Clusterização Hierárquica** | Implementação do algoritmo aglomerativo. Foco nos diferentes **Critérios de Ligação** (Single, Complete, Average, Ward) e na análise visual de **Dendrogramas** para a identificação da estrutura de clusters. |
| `04 - DBSCAN.ipynb` | **DBSCAN** | Implementação e análise do algoritmo *DBSCAN* (baseado em densidade). Inclui a detecção de *outliers* (ruído), a técnica **K-Distance** para estimação do $\varepsilon$ (epsilon) e a aplicação em séries temporais com a métrica **DTW** (Dynamic Time Warping). |

## ✨ Destaques de Implementação

* **Implementação do Zero:** Os notebooks `K-Means` e `Hierarchical` contêm classes construídas do zero (`KMeans` e `HierarchicalClustering`), utilizando apenas a biblioteca NumPy para fins educacionais, demonstrando o funcionamento interno dos algoritmos.
* **Análise de Métricas:** Uso de métricas como **Inércia (WCSS)**, **Pureza do Cluster** e técnicas como o **Gráfico de Pares (Pair Plot)** e **K-Distance Plot** para justificar a seleção de features e parâmetros.
* **Métricas de Distância Customizadas:** O notebook de DBSCAN explora o uso de métricas de distância não euclidianas, como a **Distância Radial** e o **DTW**, para resolver problemas de clusterização que metódos tradicionais não conseguem abordar.

## 🛠️ Tecnologias Utilizadas

* **Python 3.x**
* **NumPy:** Para manipulação de dados e implementação das funções centrais.
* **Matplotlib / Seaborn / Plotly:** Para visualização dos dados, clusters, centróides e dendrogramas.
* **Scikit-learn (sklearn):** Para carregamento de datasets (Iris, Wine) e comparação de resultados.
* **SciPy:** Para as funções otimizadas de Clusterização Hierárquica (`linkage`, `dendrogram`, `fcluster`).
* **Dtaidistance:** Utilizada para o cálculo da distância DTW (Dynamic Time Warping) em séries temporais.
