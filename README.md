# Pipeline ETL com IA Generativa - Análise de Churn Bancário

Este projeto foi desenvolvido como parte de um desafio prático de Ciência de Dados. O objetivo é demonstrar um fluxo completo de ETL (Extração, Transformação e Carga) enriquecido com Inteligência Artificial (Gemini) para apoiar gerentes de contas na retenção de clientes.

## 🛠️ O Desafio

Construir um pipeline que analisa uma base de clientes bancários, identifica perfis de risco de evasão (Churn) e gera, automaticamente, planos de ação personalizados para o gerente da conta.

## 🚀 Tecnologias Utilizadas

* **Python:** Linguagem principal para o script de ETL.
* **Google Gemini (via API):** IA Generativa utilizada para criar as análises qualitativas e sugestões de ação.
* **Pandas/JSON:** Manipulação de dados.
* **HTML/JS:** Frontend para visualização dos resultados.

## ⚙️ Arquitetura do ETL - Google Colab

Veja o arquivo **DesafioETLPython.ipynb**

1.  **Extract (Extração):** Simulação de uma base de dados JSON com 20 clientes (divididos entre: Já Cancelados, Em Risco e Normais).
2.  **Transform (Transformação):** * Filtragem de clientes.
    * Integração com a API do Google Gemini.
    * Para clientes em **Risco**, a IA sugere ações de retenção imediatas.
    * Para clientes **Normais**, a IA projeta oportunidades de investimento.
3.  **Load (Carga):** Os dados enriquecidos são salvos em um novo arquivo `clientes_analisados.json` pronto para consumo pelo Dashboard Web.

## 📊 Como visualizar

Acesse o arquivo [index.html](https://a-r-soares.github.io/desafio_etl_python/) ou a página publicada no GitHub Pages para interagir com o relatório, filtrar por status (Normal, Risco, Churn) e ler as recomendações da IA.
