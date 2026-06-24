# 📊 Inteligência Educacional & Desigualdade: Microdados ENEM 2020–2023

![ENEM 2020-2023](https://img.shields.io/badge/ENEM-2020--2023-1E5EFF?style=for-the-badge)
![Fonte INEP](https://img.shields.io/badge/Fonte-INEP-00C48C?style=for-the-badge)
![Municípios](https://img.shields.io/badge/Municípios-5.570-FF8A00?style=for-the-badge)
![Licença](https://img.shields.io/badge/Licença-MIT-blue?style=for-the-badge)

Ecosystema analítico avançado que transforma **13,9 milhões de registros** dos Microdados do ENEM em inteligência territorial e preditiva, desenhado estrategicamente para gestores públicos, ONGs educacionais e formuladores de políticas públicas.

---

## 🎯 Links Rápidos de Acesso

* 🌐 **ENEM Vision (Inteligência Territorial):** [Acessar Plataforma](https://enem-vision.lovable.app/)
* 🔮 **Predict Edu Impact (Modelagem Preditiva):** [Acessar Plataforma](https://predict-edu-impact.lovable.app/)

---

## 🗺️ Visão Geral do Ecossistema

O projeto é composto por duas aplicações complementares que cobrem o ciclo completo de análise de dados educacionais — indo do diagnóstico descritivo à projeção preditiva de cenários.

### 1. 📊 ENEM Vision
* **Propósito:** Inteligência territorial descritiva. Conecta desempenho, renda, infraestrutura e contexto social por município, estado e região.
* **Recursos:** Mapas interativos, rankings nacionais, séries temporais, radar por área do conhecimento e distribuições estatísticas avançadas (mediana, quartis e *outliers*).
* **Cobertura:** 13,9 milhões de participantes, 1.747 municípios, mais de 40 mil escolas ao longo de 4 anos de dados, além do cálculo do IED (Índice de Esforço Docente) médio nacional fixado em 70.
* **Módulos:** 🔀 [Explorar](https://enem-vision.lovable.app/explorar) | 🏆 [Ranking](https://enem-vision.lovable.app/ranking) | 📖 [Metodologia](https://enem-vision.lovable.app/metodologia)

### 2. 🔮 Predict Edu Impact
* **Propósito:** Inteligência preditiva e simulação de cenários. Modelagem estatística da nota média do ENEM sob horizontes temporais de 2026 e 2030.
* **Recursos:** Classificação automatizada de municípios em quatro status críticos (*Referência, Estável, Atenção, Crítico*), simulador de políticas públicas impacto-resposta, radar de vulnerabilidade e motor de recomendação prescritiva baseado no **IPEE (Índice de Potencial de Evolução Educacional)**.
* **Performance do Modelo:** Erro Absoluto Médio (MAE) de 32,7 pontos, evolução estadual projetada de +7,92 pontos ao ano e 95 municípios em estado crítico (nota < 480) já mapeados.

💡 **Fluxo de Uso Recomendado:** Comece pelo **ENEM Vision** para diagnosticar o território atual (*onde está a desigualdade hoje?*), e avance para o **Predict Edu Impact** para projetar cenários e priorizar intervenções (*onde investir para maximizar o impacto até 2030?*).

---

## 🧠 Problema & Motivação

O Brasil possui o **maior banco de dados educacional da América Latina**: os Microdados do ENEM, publicados anualmente pelo INEP com dezenas de variáveis por candidato. Apesar dessa imensa riqueza informacional, esses dados historicamente permanecem inacessíveis para a tomada de decisão ágil devido a três gargalos principais:

1. **Volume e Complexidade:** Cada edição do ENEM gera arquivos brutos com mais de 3 GB e milhões de linhas em formatos complexos de processar.
2. **Falta de Territorialização:** Os dados existem no nível individual, mas não eram sistematicamente agregados e tratados por município para permitir comparações regionais diretas.
3. **Ausência de Cruzamento de Dados:** Desempenho, infraestrutura escolar e dados socioeconômicos raramente são analisados em conjunto de forma preditiva.

O **ENEM Vision** resolve os dois primeiros pontos entregando territorialização e cruzamento em tempo real. O **Predict Edu Impact** soluciona o terceiro ponto, transformando o diagnóstico estático em **previsão e recomendação acionável**.

---

## 🛠️ Stack Tecnológica & Engenharia de Dados

Para sustentar o processamento de milhões de registros com alta performance na web, o ecossistema utiliza arquitetura moderna de Data Science:

* **Processamento e Modelagem:** Python, Pandas, Scikit-Learn, Statsmodels.
* **Pipeline de Dados:** Clusterização (K-Means/Hierárquica) para classificação de vulnerabilidade e Regressões Avançadas para projeções de séries temporais.
* **Interface e Visualização:** Dashboards analíticos integrados com motores de renderização geoespacial (Mapbox/Leaflet).

---

## 👥 Autores e Responsáveis

Este ecossistema de dados foi idealizado, modelado e desenvolvido por especialistas seniores:

* 👩‍💻 **Gisele Pereira Monteiro** — *Cientista de Dados & Especialista em Modelagem*
* 👩‍💻 **Jessica Dias Sabino** — *Engenheira de Dados & Arquitetura de Pipeline*
* 👨‍💻 **Lucas de Moura Melo** — *Analista de BI & Especialista em Políticas Públicas*
* 👩‍💻 **Thays Porto de Jesus Cambi** — *Engenheira de Software & Integração de Sistemas*


