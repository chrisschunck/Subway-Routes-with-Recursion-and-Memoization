# Checkpoint 2 — Dynamic Programming: Rotas de Metrô

**Disciplina:** FIAP - Dynamic Programming  
**Checkpoint:** Checkpoint 2 — Rotas de Metrô com Recursão e Memoização

## Integrantes do Grupo

| Nome Completo | RM

Christian Schunck de Almeida| RM-563850 

Guilherme Vilela Perez | RM-564422 

Gustavo Panham Dourado | RM-563904

Paulo Cesar de Govea Junior | RM-566034 

Thomas Jeserfon Santana Wang | RM-565104 

## Estrutura do Repositório

```
Checkpoint_2_em_grupo/
├── notebook.ipynb              ← Notebook principal (executado)
├── mapa_saopaulo.html          ← Mapa interativo São Paulo
├── mapa_beijing.html           ← Mapa interativo Beijing
├── mapa_sanfrancisco.html      ← Mapa interativo San Francisco BART
├── desempenho.png              ← Gráfico comparativo com/sem memoização
└── README.md                   ← Este arquivo
```

## O que foi implementado

- **3 grafos ponderados não-dirigidos** (≥15 nós cada): Beijing (L1/L2/L4/L10), San Francisco (BART) e São Paulo (Metrô+CPTM)
- **Recursão + memoização** (`functools.lru_cache`) para o caminho mais curto
- **Backtracking** para o caminho mais longo simples (sem ciclos)
- **4 faixas de horário** com fatores ×0,6 / ×1,5 / ×1,0 / ×2,0
- **Análise de desempenho** com `tracemalloc` e `time.perf_counter`
- **Visualização com Folium** — mapas interativos com caminhos destacados

## Como executar

```bash
pip install folium nbformat matplotlib
jupyter notebook notebook.ipynb
```

## Link para o Notebook

[https://github.com/chrisschunck/Subway-Routes-with-Recursion-and-Memoization.git](https://github.com/chrisschunck/Subway-Routes-with-Recursion-and-Memoization/blob/main/notebook.ipynb)
[notebook.ipynb](./notebook.ipynb)
