# 📊 Inteligência Educacional & Desigualdade — Microdados ENEM 2020–2023
<div align="center">
![Banner](https://img.shields.io/badge/ENEM-2020--2023-1E5EFF?style=for-the-badge)
![INEP](https://img.shields.io/badge/Fonte-INEP%2FMEC-00C48C?style=for-the-badge)
![Municípios](https://img.shields.io/badge/Municípios-5.570-FF8A00?style=for-the-badge)
![Licença](https://img.shields.io/badge/Licença-MIT-blue?style=for-the-badge)
<p align="center">
  <a href="#-visão-geral">Visão Geral</a> •
  <a href="#-plataformas-desenvolvidas">Plataformas</a> •
  <a href="#-autores-e-responsáveis">Autores</a> •
  <a href="#-funcionalidades">Funcionalidades</a> •
  <a href="#-como-executar">Como Executar</a> •
  <a href="#-metodologia">Metodologia</a> •
  <a href="#-roadmap">Roadmap</a>
</p>
**Ecossistema analítico que transforma 13,9 milhões de registros dos Microdados ENEM em inteligência territorial e preditiva para gestores públicos, ONGs educacionais e formuladores de políticas públicas.**
</div>
---
## 🔗 Plataformas Desenvolvidas
Este projeto é composto por **duas aplicações complementares**, que juntas cobrem o ciclo completo de análise educacional — do diagnóstico descritivo à projeção preditiva de cenários.
<table>
<thead>
<tr>
<th align="left">Plataforma</th>
<th align="left">Propósito</th>
<th align="center">Acesso</th>
</tr>
</thead>
<tbody>
<tr>
<td>
### 🌎 ENEM Vision
**Inteligência territorial descritiva**
</td>
<td>
Plataforma de exploração interativa dos microdados ENEM 2020–2023. Conecta **desempenho, renda, infraestrutura e contexto social** por município, estado e região — com mapa inteligente, ranking nacional, séries temporais, radar por área do conhecimento e distribuições com mediana, quartis e outliers.
**Cobertura:** 13,9 mi participantes · 1.747 municípios · 40 mil+ escolas · 4 anos de dados · IED médio nacional 70.
</td>
<td align="center">
[🚀 Acessar](https://enem-vision.lovable.app/)
[📍 Explorar](https://enem-vision.lovable.app/explorar)<br>
[🏆 Ranking](https://enem-vision.lovable.app/ranking)<br>
[📖 Metodologia](https://enem-vision.lovable.app/metodologia)
</td>
</tr>
<tr>
<td>
### 🔮 Predict Edu Impact
**Inteligência preditiva & simulação de cenários**
</td>
<td>
Plataforma de **modelagem preditiva** da nota média do ENEM em horizontes de 2026 e 2030, com classificação automática de municípios em quatro status (**Referência · Estável · Atenção · Crítico**), simulador de políticas públicas, radar de vulnerabilidade e motor de recomendação baseado no índice **IPEE** (Índice de Potencial de Evolução Educacional).
**Performance do modelo:** erro absoluto médio de 32,7 pts · evolução estadual projetada de +7,92 pts/ano · 95 municípios em estado crítico identificados (nota < 480).
</td>
<td align="center">
[🚀 Acessar](https://predict-edu-impact.lovable.app/)
Panorama · Previsão<br>
Distribuição · Ranking<br>
Simulador · Radar<br>
Recomendação · IPEE
</td>
</tr>
</tbody>
</table>
> 💡 **Fluxo de uso recomendado:** comece pelo **ENEM Vision** para diagnosticar o território (onde está a desigualdade hoje?), e avance para o **Predict Edu Impact** para projetar cenários e priorizar intervenções (onde investir para maximizar o impacto até 2030?).
---
## 🗺️ Navegação Rápida
| Seção | Conteúdo | Link Direto |
| :--- | :--- | :---: |
| 🔗 **Plataformas** | Acesso direto às duas ferramentas | [Acessar](#-plataformas-desenvolvidas) |
| 👥 **Equipe** | Autores e responsáveis pelo projeto | [Acessar](#-autores-e-responsáveis) |
| 🚀 **Primeiros Passos** | Como instalar e rodar o projeto localmente | [Acessar](#-como-executar) |
| 📊 **Módulos** | Funcionalidades, IED, IPEE e análise socioeconômica | [Acessar](#-funcionalidades) |
| 🔬 **Ciência de Dados** | Modelos estatísticos, regressão e clusterização | [Acessar](#-módulos-analíticos) |
<details>
<summary><b>📐 Clique aqui para ver o Índice Completo do Projeto</b></summary>
- [Visão Geral](#-visão-geral)
- [Plataformas Desenvolvidas](#-plataformas-desenvolvidas)
- [Autores e Responsáveis](#-autores-e-responsáveis)
- [Problema e Motivação](#-problema-e-motivação)
- [Funcionalidades](#-funcionalidades)
- [Arquitetura do Sistema](#️-arquitetura-do-sistema)
- [Stack Tecnológica](#-stack-tecnológica)
- [Estrutura do Projeto](#-estrutura-do-projeto)
- [Base de Dados](#-base-de-dados)
- [Índice IED](#-índice-ied--inteligência-educacional-e-desigualdade)
- [Índice IPEE](#-índice-ipee--potencial-de-evolução-educacional)
- [Módulos Analíticos](#-módulos-analíticos)
- [Como Executar](#-como-executar)
- [Variáveis de Ambiente](#-variáveis-de-ambiente)
- [API Reference](#-api-reference)
- [Metodologia](#-metodologia)
- [Casos de Uso](#-casos-de-uso)
- [Roadmap](#-roadmap)
- [Contribuição](#-contribuição)
- [Licença](#-licença)
</details>
---
## 🚨 Problema e Motivação
O Brasil possui **o maior banco de dados educacional da América Latina**: os Microdados do ENEM, publicados anualmente pelo INEP com dezenas de variáveis por candidato. Apesar da riqueza informacional, esses dados permanecem inacessíveis para a maioria dos gestores públicos e formuladores de política educacional por três razões principais:
1. **Volume e complexidade**: cada edição do ENEM gera arquivos com mais de 3 GB e milhões de linhas em formato bruto.
2. **Falta de territorialização**: os dados existem no nível individual, mas não são sistematicamente agregados por município para comparação regional.
3. **Ausência de cruzamento**: desempenho, infraestrutura e renda raramente são analisados em conjunto na tomada de decisão pública — e quase nunca são projetados em cenários futuros.
O **ENEM Vision** ataca os dois primeiros pontos, entregando territorialização e cruzamento em tempo real. O **Predict Edu Impact** ataca o terceiro, transformando o diagnóstico em **previsão e recomendação acionável** até 2030.
---
## 👥 Autores e Responsáveis
Este projeto foi idealizado e desenvolvido por:
* **Gisele Pereira Monteiro**
* **Jessica Dias Sabino**
* **Lucas de Moura Melo**
* **Thays Porto de Jesus Cambi**


