# TT12 – Trending Videos Dashboard

Este projeto consiste no desenvolvimento de um **dashboard analítico** para monitorar vídeos em tendência no YouTube, com foco em apoiar decisões de marketing na agência **Sterling & Draper**.

O objetivo central é:

> Identificar padrões de conteúdo em alta para orientar investimentos em campanhas publicitárias.

---

## 🎯 Objetivo de Negócio

Automatizar a análise de vídeos em tendência para responder, de forma rápida e recorrente:

- Quais categorias estão em alta?
- Como essas tendências variam por região?
- Quais conteúdos têm maior potencial nos EUA?

---

## 🔍 Descrição do Projeto

O projeto foi estruturado para transformar dados brutos em um **dashboard interativo**, utilizado diariamente por gestores de marketing.

### Principais entregáveis:

- Dashboard com análise temporal de tendências
- Distribuição de vídeos por região
- Correspondência entre categorias e países
- Filtros dinâmicos por data e localização

---

## 📊 Estrutura do Dashboard

O dashboard é composto por quatro blocos principais:

### 1. Histórico de Tendências (Valores Absolutos)

- Gráfico de área empilhada
- Eixo X: tempo (data de trending)
- Eixo Y: volume de vídeos (`videos_count`)
- Segmentação por categoria

Objetivo:
Visualizar evolução e volume total de tendências ao longo do tempo.

---

### 2. Histórico de Tendências (%)

- Gráfico de área empilhada percentual
- Mostra a participação relativa de cada categoria

Objetivo:
Identificar mudanças de relevância entre categorias.

---

### 3. Distribuição por País

- Gráfico de pizza (%)
- Participação de cada região no total de vídeos

Insight observado:
Distribuição relativamente equilibrada, com exceção de uma região com menor representatividade.

---

### 4. Correspondência Categoria × País

- Tabela agregada
- Valores absolutos por categoria e região

Objetivo:
Permitir análises cruzadas e identificação de padrões regionais.

---

## 🧠 Principais Insights

### 📌 Categorias mais frequentes

- Entertainment  
- People & Blogs  
- Music  
- News & Politics  

---

### 📌 Distribuição regional

- Estados Unidos lideram levemente
- Japão apresenta menor volume relativo

---

### 📌 Destaque nos Estados Unidos

Categorias mais relevantes:

- Entertainment  
- Music  
- Howto & Style  
- Comedy  
- People & Blogs  

---

### 📌 Diferenças regionais

- **News & Politics** é mais forte fora dos EUA  
- **Howto & Style** é mais relevante nos EUA  

---

## 🗂️ Fonte de Dados

Tabela agregada:

`trending_by_time`

Campos:

- `record_id` — identificador único  
- `region` — país/região  
- `trending_date` — data/hora  
- `category_title` — categoria  
- `videos_count` — número de vídeos  

Banco de dados: `youtube`

Atualização: **diária (UTC 00:00)**

---

## ⚙️ Funcionalidades do Dashboard

- Filtro por intervalo de data
- Filtro por região
- Interação dinâmica entre todos os gráficos
- Visualização integrada (tempo + categoria + país)

---

## 🚀 Tecnologias Utilizadas

- SQL (extração e agregação)
- Tableau / Power BI (visualização)
- Modelagem de dados agregados

---

## 📦 Como Executar

1. Clone o repositório:

```bash
git clone https://github.com/rodriguesbrian/tt12_trending_videos.git
cd tt12_trending_videos