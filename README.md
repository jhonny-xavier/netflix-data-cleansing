# Netflix Data Analysis — Limpeza de Dados e EDA
Ferramentas: Python (Pandas) · SQL · Tableau Public
Dataset: 8.807 títulos | Fonte: Kaggle Netflix Movies and TV Shows

📌 Visão Geral
Projeto de análise de dados end-to-end focado em resolver inconsistências reais em um
dataset de produção, construindo um pipeline de limpeza reproduzível e um dashboard
interativo para exploração de tendências de conteúdo da Netflix.

🎯 Problema de Negócio
O campo `duration` misturava duas unidades distintas ('90 min' para filmes e '2 Seasons'
para séries), tornando qualquer agregação direta matematicamente inválida.
Solução: separação condicional em dois campos numéricos independentes,
eliminando distorções nos agregados e habilitando comparações corretas por tipo.

🛠️ Decisões Técnicas por Ferramenta
Cada ferramenta foi escolhida para o estágio onde oferece maior produtividade:

- SQL: transformações na camada de dados — CASE WHEN para parsing condicional
  de strings e conversão de tipo. Escolhido por performance em grandes volumes.

- Python/Pandas: EDA exploratória e engenharia de features — np.where() para
  atribuição condicional vetorizada; indexação booleana df[df['type']=='Movie']
  para filtragem eficiente de subconjuntos. Escolhido pela flexibilidade analítica.

- Tableau: visualização final para stakeholders não técnicos — IF e SPLIT para
  separação lógica em nível de linha. Escolhido pela acessibilidade do dashboard.

📊 Insights Encontrados na EDA
- Concentração geográfica: 36% do catálogo é produção americana; Índia (12%) e
  Reino Unido (8%) formam os outros dois maiores polos — dado relevante para
  estratégia de diversificação regional.
- Aceleração do catálogo: entre 2015 e 2019 a adição de títulos cresceu 280%,
  com queda em 2020-2021 possivelmente relacionada à pandemia.
- Proporção Filmes vs Séries: 69% filmes, 31% séries — distribuição que sugere
  foco histórico em cinema com crescimento recente de séries originais.
- Gêneros dominantes: Drama Internacional e Comédia lideram; Documentários
  representam segmento menor mas com crescimento acelerado desde 2017.

🔗 Dashboard Interativo
Publicado no Tableau Public com filtros globais por Ano de Lançamento e Diretor,
permitindo segmentação dinâmica do catálogo completo.

👉 **[Click here to access the Live Tableau Dashboard]https://public.tableau.com/app/profile/jhonny.machado/viz/Livro1_17805904090720/Dashboard2?publish=yes**

---
*Project built as part of my Data Analytics continuous learning journey.*
<img width="1363" height="764" alt="Dash" src="https://github.com/user-attachments/assets/421eaf92-9d22-44ec-a6c2-6d6943429049" />


---
*Project built as part of my Data Analytics continuous learning journey.*
