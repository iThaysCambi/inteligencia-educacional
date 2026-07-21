# 📊 Inteligência Educacional & Desigualdade: Microdados ENEM · SP (2015–2023)

[![Status do Projeto](https://img.shields.io/badge/Status-Conclu%C3%ADdo-00C48C?style=for-the-badge)](#)
[![ENEM 2015-2023](https://img.shields.io/badge/ENEM-2015--2023-1E5EFF?style=for-the-badge)](#)
[![Municípios SP](https://img.shields.io/badge/Munic%C3%ADpios%20SP-643-FF8A00?style=for-the-badge)](#)
[![Power BI](https://img.shields.io/badge/Power_BI-Desktop-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](#)
[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)](#)
[![MySQL](https://img.shields.io/badge/MySQL-Data_Warehouse-4479A1?style=for-the-badge&logo=mysql&logoColor=white)](#)

> **Resumo Executivo:** Um ecossistema analítico completo que processa **mais de 5,2 milhões de registros** dos Microdados do ENEM para diagnosticar disparidades socioeconômicas e prever o desempenho educacional até 2030 em 643 municípios paulistas. Integrando pipeline ETL, Data Warehouse, BI e aplicação web preditiva.

---

## 🎯 Entregáveis do Projeto & Links de Acesso

| Entregável | Descrição / Objetivo | Link de Acesso / Ação |
| :--- | :--- | :--- |
| 🔮 **Web App Preditivo (IPEE)** | Aplicação Web para simulação de cenários educacionais (2024–2030) | [![Acessar App](https://img.shields.io/badge/Acessar_Plataforma-Lovable-7C3AED?style=for-the-badge&logo=react)](https://predict-edu-impact.lovable.app/) |
| 📥 **Arquivo do Power BI (.pbix)** | Relatório completo com modelo de dados DAX, visuais e filtros | [![Download .pbix](https://img.shields.io/badge/Download-ENEM.pbix-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](<a href="https://seu-link-do-onedrive-aqui" target="_blank">
  <img src="https://img.shields.io/badge/DOWNLOAD-ENEM.PBIX-yellow?style=for-the-badge" alt="Download Power BI">
</a>) |
| 💻 **Código Fonte ETL** | Scripts de higienização, engenharia de atributos e carga MySQL | [![Ver Código](https://img.shields.io/badge/Reposit%C3%B3rio-Código_Python-3776AB?style=for-the-badge&logo=github)](#-engenharia-de-dados--arquitetura-técnica) |

---

## 🗺️ Visão Geral da Solução

O ecossistema resolve a dor da **tomada de decisão no escuro em gestão pública** unindo inteligência descritiva e modelagem estatística preditiva.
---
┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐
│  Microdados     │ ──> │   ETL Python    │ ──> │  Data Warehouse │ ──> │   Entregáveis   │
│  INEP 2015-2023 │     │  Pandas/Limpeza │     │  MySQL (Fato/Dim)│     │ Power BI + App  │
└─────────────────┘     └─────────────────┘     └─────────────────┘     └─────────────────┘

### 1. 📊 Dashboard Analítico em Power BI (`ENEM.pbix`)
Desenvolvido focado em **Storytelling com Dados** para gestores de educação e analistas de BI:
* **Painel Demográfico:** Mapeamento de 5,2M+ participantes por raça/cor (54% pretos/pardos, 42% brancos), gênero e distribuição de faixas de renda.
* **Análise Temporal (Real vs. Previsto):** Séries temporais de 2015 a 2023 para as 4 áreas de conhecimento (Matemática, Humanas, Linguagens e Natureza) comparando notas reais com a regressão estimada.
* **Matriz de Dispersão Socioeconômica:** Cruzamento direto entre Renda Média Familiar e Notas com filtros dinâmicos por Ano e Região (Grande SP, Campinas e Região, Interior SP, SP Capital).

### 2. 🔮 Plataforma Web Preditiva — IPEE (Predict Edu Impact)
Interface voltada para formuladores de políticas públicas com **7 módulos interativos**:
* **Panorama:** Comparativo da nota média do estado (532 em 2023 ➔ projeção de 587,6 em 2030).
* **Mapeamento de Criticidade:** Identificação e classificação automática de **95 municípios em estado crítico** (nota média < 480).
* **Simulador de Intervenção & Recomendador:** Algoritmo que projeta o ganho de pontuação com base em investimentos prioritários em infraestrutura e redes escolares.

---

## 💡 Key Business Insights

1. **Impacto da Renda ($R^2 = 0,74$):** Candidatos de municípios com renda familiar superior a R$ 2.000,00 apresentam notas **15% superiores** em exatas e redação.
2. **Disparidade Racial & Territorial:** Candidatos pretos e pardos somam 54% dos inscritos, mas estão concentrados em regiões de menor rendimento, gerando um gap de desempenho histórico de até **80 pontos em Matemática**.
3. **Poder Preditivo Acurado:** O modelo de Regressão Linear atingiu um **Erro Absoluto Médio (MAE) de apenas 32,7 pontos** sobre as médias municipais acumuladas.

---

## 🛠️ Engenharia de Dados & Arquitetura Técnica

* **Processamento & ETL:** Python (Pandas) para ingestão e limpeza de arquivos pesados, agregação geográfica por código IBGE e tratamento de omissões socioeconômicas.
* **Modelagem Relacional:** Data Warehouse em MySQL modelado em **Star Schema** (Tabela Fato `forecast_2015_2023` conectada às dimensões `dim_municipios` e `dim_socioeconomico`).
* **Data Science:** Algoritmos de Regressão Linear e Séries Temporais para projeções com validação cruzada.
* **Business Intelligence:** Power BI Desktop utilizando linguagem DAX para cálculo de métricas agregadas e design acessível.

---

## 📥 Como Avaliar o Projeto Localmente

### Pré-requisitos
* [Power BI Desktop](https://powerbi.microsoft.com/) instalado no Windows.

### Passo a Passo
1. Faça o download do arquivo do projeto:
   * 📁 [Baixar ENEM.pbix via Google Drive]("<a href="https://seu-link-do-onedrive-aqui" target="_blank">
  <img src="https://img.shields.io/badge/DOWNLOAD-ENEM.PBIX-yellow?style=for-the-badge" alt="Download Power BI">
</a>")
2. Abra o arquivo no **Power BI Desktop**.
3. Utilize os navegadores de páginas no rodapé (`Inf. Demo.`, `Info. Analises`, `Renda vs Notas`) para explorar a interatividade dos dados.

---

## 👥 Autores & Contribuidores

Este ecossistema de dados foi idealizado, modelado e desenvolvido por Analista de Dados:

* 👩‍💻 **Gisele Pereira Monteiro** 
* 👩‍💻 **Jessica Dias Sabino** 
* 👨‍💻 **Lucas de Moura Melo**  
* 👩‍💻 **Thays Porto de Jesus Cambi** 


