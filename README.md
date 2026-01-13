# 📊 Dashboard Futura | Gestão de Operações

![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![Streamlit](https://img.shields.io/badge/Frontend-Streamlit-FF4B4B)
![Plotly](https://img.shields.io/badge/Viz-Plotly-3F4F75)
![Supabase](https://img.shields.io/badge/Database-Supabase-3ECF8E)

## 📋 Sobre o Projeto

O **Dashboard Futura** é uma solução de Business Intelligence (BI) desenvolvida para monitoramento em tempo real de operações de campo e assistência técnica. O sistema centraliza dados de múltiplos projetos (Americanas, Claro, Projetos Especiais) em uma interface visual interativa.

A aplicação permite que gestores acompanhem KPIs críticos, produtividade técnica e distribuição geográfica das ordens de serviço (OS).

## ✨ Principais Funcionalidades

* **KPIs em Tempo Real:** Visualização imediata de total de chamados, pendências e conclusões.
* **Filtros Dinâmicos:** Segmentação de dados por Status, Técnico Responsável e Cidade/UF.
* **Geolocalização:** Mapa interativo plotando as ordens de serviço baseado em latitude/longitude.
* **Arquitetura Híbrida:** O sistema foi projetado para operar conectado ao **Supabase** (Nuvem) com fallback automático para planilhas locais (`.xlsx`) em caso de falha de conexão ou uso offline.
* **Análise de Desempenho:** Gráficos comparativos de produtividade por técnico.

## 🚀 Tecnologias Utilizadas

* **Frontend/App:** Streamlit
* **Processamento de Dados:** Pandas
* **Visualização:** Plotly Express
* **Banco de Dados:** Supabase (PostgreSQL) & Excel (Local Backup)

## 📦 Como Rodar Localmente

### Pré-requisitos
* Python 3.8+
* Git

### Passo a Passo

1.  **Clone o repositório**
    ```bash
    git clone [https://github.com/IoT-Luiz-Filipe99/dashboard-futura.git](https://github.com/IoT-Luiz-Filipe99/dashboard-futura.git)
    cd dashboard-futura
    ```

2.  **Instale as dependências**
    ```bash
    pip install -r requirements.txt
    ```

3.  **Configuração (Opcional)**
    Para conectar ao banco de dados em nuvem, crie um arquivo `.env` ou `secrets.toml` com suas credenciais do Supabase. Caso contrário, o sistema usará automaticamente o arquivo `dados_unificados.xlsx` local.

4.  **Execute o Dashboard**
    ```bash
    streamlit run dash-base-supa-juncao.py
    ```

5.  **Acesse**
    O navegador abrirá automaticamente em: `http://localhost:8501`

## 📷 Screenshots

*(Recomendado: Adicione aqui um print da tela do seu dashboard rodando)*

## 📄 Licença

Este projeto está sob a licença MIT.