# Modelagem de Risco de Crédito com XGBoost e análise SHAP

## 📌 Contexto de Negócio
Este projeto desenvolve um modelo estatístico para estimar a probabilidade de incumprimento (*default*) de clientes de cartão de crédito. Com base em variáveis de comportamento financeiro e histórico de pagamentos, a solução visa otimizar as políticas de concessão de crédito, maximizando a segurança do portefólio sem recorrer a variáveis demográficas (garantindo ausência de viés discriminatório).

## 🚀 Impacto e Métricas
O modelo treinado prioriza a interceção eficaz de perfis de alto risco e apresenta indicadores validados pelos padrões do mercado financeiro:
* **Estatística KS2:** `42.38%` (Capacidade de separação excelente, isolando o risco nos decis mais altos).
* **AUC-ROC:** `0.7816` (Elevado poder de discriminação global).
* **Explicabilidade:** Implementação de `SHAP` values para garantir total transparência algorítmica e permitir auditorias precisas sobre os motivos que influenciam o agravamento do risco do cliente.

## 🛠️ Tecnologias Utilizadas
* **Linguagem:** Python 3.x
* **Machine Learning:** Scikit-Learn, XGBoost
* **Data Prep & EDA:** Pandas, Numpy, Matplotlib, Seaborn
* **Model Explainability:** SHAP

## 📂 Estrutura do Projeto e Dados
Os dados utilizados são referentes à base "Default of Credit Card Clients" (Taiwan). Por questões de conformidade e boas práticas, o ficheiro `.csv` original não está versionado neste repositório. 

Para reproduzir este projeto localmente:
1. Faça o clone do repositório.
2. Instale as dependências: `pip install -r requirements.txt`.
3. Descarregue a base de dados original [Default of Credit Card Clients Dataset](https://www.kaggle.com/datasets/uciml/default-of-credit-card-clients-dataset?resource=download) e guarde-a na pasta `data/` com o nome `default_credit_card_clients.csv`.
4. Execute as células do `main.ipynb`.