# 📊 Inteligência Educacional & Desigualdade: Microdados ENEM · SP (2015–2023)

![ENEM 2015-2023](https://img.shields.io/badge/ENEM-2015--2023-1E5EFF?style=for-the-badge)
![Fonte INEP](https://img.shields.io/badge/Fonte-INEP-00C48C?style=for-the-badge)
![Municípios SP](https://img.shields.io/badge/Munic%C3%ADpios%20SP-643-FF8A00?style=for-the-badge)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Licença](https://img.shields.io/badge/Licen%C3%A7a-MIT-blue?style=for-the-badge)

Ecossistema analítico avançado de dados que transforma **mais de 5,2 milhões de registros** dos Microdados do ENEM (2015–2023) em inteligência territorial e preditiva. O projeto conecta ETL em Python, Data Warehouse em MySQL, visualização no Power BI e uma aplicação Web Preditiva (IPEE) para gestores públicos, ONGs e tomadores de decisão.

---

## 🎯 Links Rápidos & Entregáveis

* 🔮 **Predict Edu Impact (Web App IPEE)** — [![Deploy](https://img.shields.io/badge/Acessar%20Plataforma-Lovable-blueviolet)](https://predict-edu-impact.lovable.app/)
* 📊 **Dashboard Interativo Power BI** — [![Power BI Service](https://img.shields.io/badge/Acessar%20Dashboard-Power_BI-yellow)](https://app.powerbi.com/view?r=SEU_LINK_GERADO_AQUI)
* 📥 **Download do Arquivo Power BI (.pbix)** — [![Power BI File](https://img.shields.io/badge/Download-ENEM.pbix-F2C811?logo=powerbi&logoColor=black)](./ENEM.pbix)

---
┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐
│  Microdados     │ ──> │   ETL Python    │ ──> │  Data Warehouse │ ──> │   Entregáveis   │
│  INEP 2015-2023 │     │  Pandas/Limpeza │     │  MySQL (Fato/Dim)│     │ Power BI + App  │
└─────────────────┘     └─────────────────┘     └─────────────────┘     └─────────────────┘

## 🗺️ Visão Geral da Solução

O ecossistema é composto por duas frentes integradas que cobrem todo o ciclo de dados: do tratamento bruto à prescrição automatizada.

### 1. 📊 Dashboard Analítico (Power BI)
* **Propósito:** Diagnóstico demográfico e análise temporal/socioeconômica detalhada do desempenho no ENEM.
* **Recursos:**
  * **Painel Demográfico:** Análise por raça/cor (54% pretos e pardos, 42% brancos), gênero (57% mulheres, 43% homens) e renda.
  * **Análise Temporal (Real vs. Previsto):** Acompanhamento de séries temporais de 2015 a 2023 por disciplina (Matemática, CH, CN, LC) com validação de aderência do modelo preditivo.
  * **Renda vs. Desempenho:** Matriz de dispersão comprovando a forte correlação positiva entre renda familiar média e nota de exatas/redação.
  * **Filtros Dinâmicos:** Navegação interativa por Ano e Região Geográfica (ex: São Paulo Capital, Campinas e Região).

### 2. 🔮 Web App Preditivo: IPEE (Predict Edu Impact)
* **Propósito:** Plataforma de planejamento estratégico e simulação de cenários para o período **2024–2030** nos **643 municípios do estado de São Paulo**.
* **Módulos Principais:**
  * 📊 **Panorama:** Visão geral comparativa (Média 2023 Real: 532 pts ➔ Projeção 2030: 587,6 pts).
  * 🔮 **Previsão:** Projeção contínua da evolução das notas por município.
  * 📍 **Distribuição:** Mapa de calor de desempenho territorial.
  * 🏆 **Ranking:** Classificação por performance e evolução.
  * 🎛️ **Simulador & Radar:** Simulação de intervenções com cálculo de risco/potencial.
  * 💡 **Recomendação:** Sugestões automáticas de políticas públicas conforme a criticidade do município.

---

## 🧠 O Problema de Negócio & Insights Alcançados

O desempenho no ENEM reflete desigualdades estruturais profundas. A tomada de decisão em políticas públicas educacionais frequentemente sofre com a falta de dados territorializados e preditivos.

### Key Insights do Projeto:
1. **Desigualdade Racial & Acesso:** Candidatos pretos e pardos somam **54% dos inscritos**, porém concentram-se em regiões vulneráveis, apresentando um gap histórico de até **80 pontos** em Matemática frente a candidatos brancos.
2. **Impacto da Renda ($R^2 = 0,74$):** Municípios com renda média familiar superior a R$ 2.000,00 registram notas **15% maiores**. A rede pública representa ~85% dos candidatos e necessita de investimentos direcionados.
3. **Mapeamento de Prioridades:** O modelo identificou e mapeou **95 municípios em estado crítico** (nota média < 480) no estado de SP, direcionando onde aplicar recursos pedagógicos com urgência.

---

## 🛠️ Arquitetura de Dados & Pipeline Técnico

* **Extração & Tratamento:** Python & Pandas (limpeza de microdados multigigabyte, tratamento de nulos, categorização de faixas de renda).
* **Modelagem Relacional:** MySQL Data Warehouse (modelagem dimensional de Fatos e Dimensões socioeconômicas/geográficas).
* **Modelagem Preditiva:** Algoritmos de Regressão Linear treinados nos históricos de 2015–2023 para projeção até 2030 (**Erro Absoluto Médio / MAE: 32,7 pontos**).
* **Visualização & Deploy:** Power BI Desktop/Service + Aplicação Web com IA generativa via Lovable.

---

## 🛠️ Como Executar o Dashboard localmente

1. Faça o download do arquivo `ENEM.pbix` disponível no repositório.
2. Certifique-se de ter o **Power BI Desktop** instalado em seu computador.
3. Abra o arquivo `ENEM.pbix` para navegar pelas páginas de **Análise Demográfica**, **Real vs. Previsto** e **Renda vs. Desempenho**.

---
## 👥 Autores e Responsáveis

Este ecossistema de dados foi idealizado, modelado e desenvolvido por Analista de Dados:

* 👩‍💻 **Gisele Pereira Monteiro** 
* 👩‍💻 **Jessica Dias Sabino** 
* 👨‍💻 **Lucas de Moura Melo**  
* 👩‍💻 **Thays Porto de Jesus Cambi** 


