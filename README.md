# Análise de Evasão de Clientes (Churn) em Empresa de Telecomunicações

## 📝 1. Descrição do Projeto

Este projeto de Data Science tem como objetivo principal analisar a base de dados de clientes de uma empresa fictícia de telecomunicações, a **TelecomX**. O foco da análise é identificar os principais fatores que levam um cliente a cancelar seus serviços (fenômeno conhecido como **Churn**), a fim de propor estratégias que possam reduzir essa taxa de evasão e aumentar a retenção.

Entender os motivos do churn é crucial para a saúde financeira da empresa, pois o custo de adquirir um novo cliente é geralmente muito superior ao de manter um existente.

## 🗃️ 2. Estrutura do Repositório

O repositório está organizado da seguinte forma:

-   `TelecomX.ipynb`: Notebook Jupyter contendo todo o processo de análise, desde a importação e limpeza dos dados até a visualização e extração de insights.
-   `dados_tratados.csv`: O conjunto de dados limpo e pré-processado, pronto para análise.
-   `dados_binarios.csv`: Uma versão do dataset com variáveis categóricas convertidas para formato numérico (binário), preparada para a aplicação de algoritmos de Machine Learning.
-   `README.md`: Este arquivo, com a documentação completa do projeto.

## 🚀 3. Metodologia Aplicada

O projeto seguiu as etapas clássicas de um ciclo de vida de análise de dados:

1.  **Importação e Limpeza de Dados:** Carregamento dos dados e aplicação de tratamentos para garantir a qualidade da análise, como a conversão de tipos de dados e o tratamento de valores ausentes na coluna `TotalCharges`.
2.  **Análise Exploratória de Dados (EDA):** Investigação aprofundada dos dados para identificar padrões e correlações entre as variáveis e a variável alvo (`churn`). Foram geradas diversas visualizações (gráficos de barra, histogramas, etc.) para entender o comportamento dos clientes.
3.  **Extração de Insights:** Com base na EDA, foram identificados os perfis de clientes com maior e menor probabilidade de churn.
4.  **Recomendações Estratégicas:** Elaboração de sugestões e ações que a empresa pode tomar para mitigar os riscos de churn identificados.

## 💡 4. Principais Insights e Conclusões

A análise revelou um perfil claro do cliente com maior propensão a cancelar o serviço:

* **Tipo de Contrato:** Clientes com **contrato mensal (Month-to-month)** possuem uma taxa de churn drasticamente superior aos de contrato anual.
* **Método de Pagamento:** O pagamento via **Cheque Eletrônico (Electronic Check)** está fortemente correlacionado com uma alta taxa de evasão, enquanto métodos automáticos (Cartão de Crédito e Débito em Conta) apresentam maior retenção.
* **Cobrança Mensal:** Clientes com cobranças mensais (`MonthlyCharges`) mais elevadas tendem a cancelar mais.
* **Tempo de Contrato (Tenure):** Clientes mais novos, com pouco tempo de casa, têm uma chance muito maior de cancelar. A lealdade aumenta com o tempo.
* **Serviços de Suporte:** A contratação de serviços de valor agregado, como **Suporte Técnico (Tech Support)** e **Segurança Online (Online Security)**, diminui significativamente a probabilidade de churn.

## 🛠️ 5. Tecnologias Utilizadas

-   **Linguagem:** Python 3
-   **Bibliotecas Principais:**
    -   `Pandas`: Para manipulação e análise de dados.
    -   `Matplotlib` e `Seaborn`: Para visualização de dados e criação de gráficos.
    -   `Jupyter Notebook`: Como ambiente de desenvolvimento interativo.

## ▶️ 6. Como Executar o Projeto

Para replicar a análise, siga os passos abaixo:

1.  Clone este repositório:
    ```bash
    git clone [https://github.com/mmnasciment/telecomx_customerschurn.git](https://github.com/mmnasciment/telecomx_customerschurn.git)
    ```
2.  Navegue até o diretório do projeto:
    ```bash
    cd telecomx_customerschurn
    ```
3.  Instale as dependências necessárias (recomenda-se o uso de um ambiente virtual):
    ```bash
    pip install pandas matplotlib seaborn jupyter
    ```
4.  Abra o Jupyter Notebook:
    ```bash
    jupyter notebook TelecomX.ipynb
    ```

## 👨‍💻 7. Autor

* **Nome:** Matheus Martins
* **GitHub:** [mmnasciment](https://github.com/mmnasciment)
