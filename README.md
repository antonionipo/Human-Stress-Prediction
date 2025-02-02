# Human Stress Prediction 🧠

Este repositório contém o projeto de replicação de um modelo de **predição de stress a partir de textos**, desenvolvido no contexto do programa **Trusted Tester for Data Science Agent (DSA)** no **Google Colab**. O objetivo foi avaliar o desempenho do **Data Science Agent** replicando um projeto de nível intermediário do Kaggle, utilizando apenas informações descritivas de um repositório no GitHub.

## 📊 **Descrição do Projeto**
O projeto visa classificar textos em duas categorias:
- **Com Stress (1)**
- **Sem Stress (0)**

Os dados utilizados são oriundos do Kaggle: [Human Stress Prediction Dataset](https://www.kaggle.com/datasets/kreeshrajani/human-stress-prediction).

O processo incluiu:
1. **Análise Exploratória de Dados (EDA)**
2. **Pré-processamento de Texto**
3. **Engenharia de Atributos**
4. **Treinamento e Avaliação de Modelos de Machine Learning**

## 🤖 **Comparação de Códigos e Resultados**

Foram comparados dois notebooks:

- 🔍 **Notebook Original**: [Prevendo Stress](https://github.com/gustavoramos82/Texto-Stress)
- 🚀 **Notebook Replicado**: [Projeto Replicado](https://github.com/antonionipo/aqui)

### 🔑 **Principais Diferenças:**

1. **Abordagem de Pré-processamento:**  
   - O notebook original aplicou técnicas clássicas de limpeza de texto com *stopwords*, *stemming* e tokenização simples.  
   - O notebook replicado utilizou o Data Science Agent, otimizando etapas com sugestões de engenharia de atributos mais robustas, incluindo variáveis derivadas de *timestamps* e contagem de termos relacionados ao stress.

2. **Modelagem:**  
   - O projeto original treinou modelos como **Logistic Regression**, **KNN**, **Naive Bayes** e **CatBoost**.  
   - Na replicação, além desses modelos, foram exploradas otimizações automáticas de hiperparâmetros com o **RandomizedSearchCV**.

3. **Resultados:**  
   - **Notebook Original:** O melhor desempenho foi do **Naive Bayes (Multinomial)** com uma acurácia de **73,9%**.  
   - **Notebook Replicado:** O **SVM com kernel sigmoid** apresentou desempenho consistente, mas o **Extra Trees Classifier** se destacou após otimizações, alcançando uma acurácia de **71,7%**.

## 🧪 **Experiência com o Data Science Agent (DSA)**

Diversos prompts foram testados até obter a melhor resposta possível. Embora o DSA tenha diminuído significativamente o trabalho manual, ele foi incapaz de criar o código de forma totalmente autônoma, exigindo supervisão constante e pequenas correções ao longo do processo.

## 📈 **Conclusões**

O uso do **Data Science Agent** demonstrou eficiência em otimizar fluxos de trabalho de ciência de dados, sugerindo melhorias relevantes no pré-processamento e na modelagem. Embora as métricas finais sejam comparáveis, o processo automatizado possibilitou uma abordagem mais exploratória, evidenciando o potencial da IA no suporte à análise de dados.

## 🚀 **Como Reproduzir**
1. Clone o repositório:
   ```bash
   git clone https://github.com/antonionipo/aqui.git
   ```
2. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```
3. Execute o notebook no Google Colab para melhores resultados.

---

💡 **Links Importantes:**
- [Base de Dados do Kaggle](https://www.kaggle.com/datasets/kreeshrajani/human-stress-prediction)  
- [Instruções Originais do Projeto](https://github.com/gustavoramos82/Texto-Stress) 

