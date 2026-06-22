# 📊 Inteligência Educacional & Desigualdade — Microdados ENEM 2020–2023

<div align="center">

![Banner](https://img.shields.io/badge/ENEM-2020--2023-1E5EFF?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI+PHBhdGggZmlsbD0id2hpdGUiIGQ9Ik0xMiAyTDIgN2wxMCA1IDEwLTV6TTIgMTdsOCA0IDgtNE0yIDEybDEwIDUgMTAtNSIvPjwvc3ZnPg==)
![INEP](https://img.shields.io/badge/Fonte-INEP%2FMEC-00C48C?style=for-the-badge)
![Municípios](https://img.shields.io/badge/Municípios-5.570-FF8A00?style=for-the-badge)
![Licença](https://img.shields.io/badge/Licença-MIT-blue?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Ativo-success?style=for-the-badge)

**Plataforma analítica que transforma 13,9 milhões de registros dos Microdados ENEM in inteligência territorial para gestores públicos, ONGs educacionais e formuladores de políticas públicas.**

[🔗 Demo ao Vivo](https://preview--enem-vision.lovable.app/) · [📍 Explorar Município](https://preview--enem-vision.lovable.app/explorar) · [🏆 Ranking Nacional](https://preview--enem-vision.lovable.app/ranking) · [📖 Metodologia](https://preview--enem-vision.lovable.app/metodologia)

</div>

---
## 📋 Índice

- [Visão Geral](#visão-geral)
- [Autores e Responsáveis](#autores-e-responsáveis)
- [Problema e Motivação](#problema-e-motivação)
- [Funcionalidades](#funcionalidades)
- [Arquitetura do Sistema](#arquitetura-do-sistema)
- [Stack Tecnológica](#stack-tecnológica)
- [Estrutura do Projeto](#estrutura-do-projeto)
- [Base de Dados](#base-de-dados)
- [Índice IED](#índice-ied--inteligência-educacional-e-desigualdade)
- [Módulos Analíticos](#módulos-analíticos)
- [Como Executar](#como-executar)
- [Variáveis de Ambiente](#variáveis-de-ambiente)
- [API Reference](#api-reference)
- [Metodologia](#metodologia)
- [Casos de Uso](#casos-de-uso)
- [Roadmap](#roadmap)
- [Contribuição](#contribuição)
- [Licença](#licença)

## 🎯 Visão Geral

O **IED Platform** é uma ferramenta de análise educacional desenvolvida para gestores públicos, pesquisadores e organizações da sociedade civil que precisam **identificar onde os investimentos em educação são mais urgentes** no Brasil.

A plataforma cruza quatro dimensões de dados para cada um dos 5.570 municípios brasileiros:

| Dimensão | Indicadores-chave | Fonte |
|---|---|---|
| 📈 **Desempenho Acadêmico** | Médias por área do ENEM, série histórica, distribuição de notas | INEP — Microdados ENEM |
| 🌎 **Fatores Regionais** | Comparativo por UF, região e porte populacional | IBGE / INEP |
| 🏫 **Infraestrutura Escolar** | IQIE: internet, laboratórios, biblioteca, quadra | Censo Escolar INEP |
| 💰 **Renda Familiar** | Correlação renda × nota, perfil socioeconômico, escolaridade dos pais | Questionário Socioeconômico ENEM |

> **Período analisado:** ENEM 2020, 2021, 2022 e 2023 — 13,9 milhões de participantes.

---

## 👥 Autores e Responsáveis

Este projeto foi idealizado e desenvolvido por:

* **Jessica Dias Sabino**
* **Thays Porto de Jesus Cambi**
* **Lucas de Moura Melo**
* **Gisele Pereira Monteiro**

---

## 🚨 Problema e Motivação

O Brasil possui **o maior banco de dados educacional da América Latina**: os Microdados do ENEM, publicados anualmente pelo INEP com dezenas de variáveis por candidato. Apesar da riqueza informacional, esses dados permanecem inacessíveis para a maioria dos gestores públicos e formuladores de política educacional por três razões principais:

1. **Volume e complexidade**: cada edição do ENEM gera arquivos com mais de 3 GB e milhões de linhas em formato bruto
2. **Falta de territorialização**: os dados existem no nível individual, mas não são sistematicamente agregados por município para comparação regional
3. **Ausência de cruzamento**: desempenho, infraestrutura e renda raramente são analisados em conjunto na tomada de decisão pública

### O impacto da desigualdade em números
