# modelos-preditivos-de-churn
# 📊 Análise de Churn em Telecomunicações & Redes Neurais Artificiais

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458.svg)](https://pandas.pydata.org/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-F7931E.svg)](https://scikit-learn.org/)

Projeto prático desenvolvido para a disciplina de **Redes Neurais Artificiais (RNA)** do curso de **Sistemas de Informação (UEA)**. O trabalho contempla a análise exploratória de dados (EDA), tratamento de inconsistências, validação de hipóteses de negócio e estruturação do pipeline de pré-processamento para predição de evasão de clientes (*Telco Customer Churn*).

---

## 🎯 Objetivos do Projeto

- **Análise Exploratória de Dados (EDA):** Identificar os principais fatores comportamentais e financeiros associados ao *churn* de clientes de telecomunicações.
- **Validação de Hipóteses de Negócio:** Avaliar quantitativamente o impacto do tempo de permanência (`tenure`), custos mensais (`MonthlyCharges`), tipo de contrato (`Contract`) e pacotes de serviços agregados na retenção de clientes.
- **Engenharia de Dados & Pré-processamento:** Tratar ruídos e espaços em branco mascarados no dataset, realizar conversões numéricas coerentes e preparar as variáveis categóricas e ordinais/nominais para modelagem.

---

## 💡 Principais Insights & Hipóteses Testadas

### 1. Tempo de Permanência (`tenure`)
- A maior taxa de evasão ocorre nos **primeiros 1 a 5 meses** de contrato (*onboarding* crítico).
- Clientes que superam a barreira inicial demonstram tendência de alta retenção a longo prazo (pico de fidelidade entre 60 e 72 meses).

### 2. Tipo de Contrato (`Contract`)
- **Contratos Mensais (*Month-to-month*):** Apresentam taxa de *churn* crítica de **~42.7%**.
- **Contratos de 1 Ano / 2 Anos:** Reduzem o *churn* para **11.3%** e **2.8%**, respectivamente, comprovando a eficácia de cláusulas de permanência.

### 3. Perfil de Alta Fidelidade (Múltiplos Serviços + Dependentes + Backup Online)
- Clientes que utilizam serviços integrados e possuem dependentes apresentam uma taxa de *churn* significativamente menor (**~6% a 8%** vs. **~27%** da média do dataset).
- **Custo de Troca (*Switching Cost*):** A dependência familiar do serviço aliada ao armazenamento de dados em nuvem dificulta a migração para concorrentes.

---

## 🛠️ Tecnologias Utilizadas

- **Linguagem:** Python 3
- **Manipulação e Análise:** `pandas`, `numpy`
- **Visualização de Dados:** `matplotlib`, `seaborn`
- **Ambiente:** Jupyter Notebook / Google Colab / VS Code

---

## 📁 Estrutura do Repositório

```text
.
├── Arthur_e_Bruno_RNA_2025_2_PP1_2.ipynb  # Notebook com EDA, limpeza e código
├── Telco-Customer-Churn.csv                # Base de dados utilizada
└── README.md                               # Documentação do projeto
