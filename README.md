# 📌 **Alura Challenge - Análise de Churn de Clientes**

# 📊 Análise e Modelagem de Churn de Clientes

Este repositório contém a segunda parte de um projeto de ciência de dados focado na análise do comportamento de clientes e identificação dos fatores que influenciam a taxa de cancelamento (*churn*). O objetivo é explorar os dados, extrair insights e desenvolver um modelo preditivo para ajudar empresas a mitigar o churn e melhorar a retenção de clientes.

---

## 📌 **Objetivos do Projeto**
- 📈 Analisar padrões de cancelamento (*churn*) de clientes.
- 🔍 Identificar os principais fatores que influenciam a decisão de saída.
- 🛠️ Criar um modelo preditivo que classifica clientes com alta propensão ao churn.
- 📊 Visualizar os dados e gerar insights estratégicos.

---

## 🗂 **Dados Utilizados**
O dataset utilizado contém informações sobre clientes de uma empresa de telecomunicações. Cada linha representa um cliente e cada coluna contém atributos como:
- 📌 **Dados Pessoais**: `gender`, `SeniorCitizen`, `Partner`, `Dependents`
- 📌 **Dados Contratuais**: `tenure`, `Contract`, `PaperlessBilling`, `PaymentMethod`
- 📌 **Serviços Utilizados**: `PhoneService`, `MultipleLines`, `InternetService`, `OnlineSecurity`, `StreamingTV`, etc.
- 📌 **Gastos**: `Charges.Monthly`, `Charges.Total`
- 🎯 **Variável-Alvo**: `Churn` (se o cliente cancelou ou não)

O dataset foi carregado a partir do arquivo `df_manipulacao.csv` e tratado para análise.

---

## ⚙️ **Metodologia**
O projeto foi dividido nas seguintes etapas:

1. **Exploração e Limpeza dos Dados**
   - Carregamento do dataset e verificação de valores nulos.
   - Análise da distribuição das variáveis.
   - Tratamento de dados desbalanceados e remoção de colunas irrelevantes.

2. **Análise Exploratória de Dados (EDA)**
   - Visualização da distribuição das variáveis categóricas e numéricas.
   - Comparação entre clientes que cancelaram (`Churn = Yes`) e os que permaneceram (`Churn = No`).
   - Geração de histogramas e gráficos de dispersão para insights.

3. **Feature Engineering**
   - Criação de novas variáveis relevantes.
   - Codificação de variáveis categóricas usando `LabelEncoder`.

4. **Modelagem Preditiva**
   - Treinamento de algoritmos de machine learning para prever churn.
   - Teste de diferentes modelos para encontrar a melhor performance.
   - Avaliação do modelo utilizando métricas como **Acurácia, Recall, F1-Score e ROC-AUC**.

---

## 📊 **Alguns Insights**
🔹 **Clientes idosos têm maior taxa de churn** (alta taxa de cancelamento entre `SeniorCitizen = 1`).  
🔹 **Clientes sem suporte técnico cancelam o serviço 2x mais do que os que possuem suporte.**  
🔹 **Contratos mensais apresentam taxas de churn muito maiores** comparados a contratos anuais ou bienais.  
🔹 **Método de pagamento impacta no churn**: clientes que pagam via cheque eletrônico têm uma taxa de cancelamento muito mais alta.  
🔹 **Clientes que usam fibra ótica têm um churn significativamente alto**, sugerindo insatisfação com o serviço.  

Essas descobertas podem ser usadas para desenvolver estratégias para reduzir o churn, como oferecer incentivos para clientes de alto risco ou melhorar a qualidade do suporte técnico.

---

## 🚀 **Tecnologias Utilizadas**
- 🐍 **Linguagem**: Python  
- 📊 **Bibliotecas**: `pandas`, `numpy`, `matplotlib`, `seaborn`, `plotly`, `scikit-learn`  
- 📡 **APIs**: `requests`, `OpenAI`  
- 🤖 **Machine Learning**: Modelos supervisionados para previsão de churn  

---

## 🏆 **Resultados e Conclusões**
Após a análise exploratória e modelagem preditiva, foi possível identificar padrões que afetam a retenção de clientes. As informações obtidas podem ser utilizadas para otimizar estratégias de fidelização e prever clientes com alto risco de cancelamento.

Os modelos preditivos desenvolvidos podem foram refinados, após `SMOTE` para balanceamento de dados e treinamento, com `GridSearchCV` para otimização de hiperparâmetros.

Com base nas métricas, Logistic Regression pareceu ser uma melhor opção. Ainda que o recall tenha dado um score menor, as outras métricas estão melhores e suportam a escolha pela diferença pequena no Recall.
---

## 📌 **Como Usar este Projeto**
1. Clone este repositório:  
   ```bash
   git clone https://github.com/seu-usuario/projeto-churn.git
   ```
2. Instale as dependências necessárias:  
   ```bash
   pip install -r requirements.txt
   ```
3. Execute o notebook Jupyter para visualizar as análises:
   ```bash
   jupyter notebook Alura_Challenge_1_pt2.ipynb
   ```

---

## 📬 **Contato**
📧 Caso tenha dúvidas ou sugestões, fique à vontade para entrar em contato:  
🔗 **LinkedIn**: [Seu Perfil](https://www.linkedin.com/in/seu-perfil/)  
🔗 **GitHub**: [Seu GitHub](https://github.com/seu-usuario)  

---

Este README fornece uma visão completa e profissional do seu projeto para o GitHub. Se precisar de ajustes ou quiser incluir mais detalhes, me avise! 🚀
