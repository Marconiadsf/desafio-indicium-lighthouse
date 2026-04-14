# Desafio Técnico — Indicium Lighthouse

Solução para o desafio técnico do processo seletivo **Indicium Lighthouse 2026**, trilha Dados & IA.

## Contexto

A **LH Nautical** é uma empresa de e-commerce de produtos náuticos. O desafio consiste em organizar, tratar e analisar dados de vendas, produtos, clientes e custos de importação, gerando insights acionáveis e modelos preditivos para apoiar decisões de negócio.

## Estrutura do Projeto

```
.
├── src/
│   └── desafio_completo.ipynb   # Notebook principal com toda a solução
├── data_input/
│   ├── vendas_2023_2024.csv     # Histórico de vendas
│   ├── produtos_raw.csv         # Catálogo de produtos
│   └── custos_importacao.json   # Custos de importação por produto
├── data_output/                 # Outputs gerados pela execução do notebook
└── media/
    ├── custos_importacao.png
    └── lh_nautical_material_executivo.pdf
```

## Solução

O notebook está organizado em 9 seções:

| Seção | Conteúdo |
|---|---|
| 0 | Configuração do ambiente e carregamento dos dados |
| 1 | Análise exploratória de vendas (EDA, qualidade, interpretação) |
| 2 | Limpeza e padronização do catálogo de produtos |
| 3 | Normalização dos dados de custos de importação |
| 4 | Análise de receita, prejuízo e dados públicos (câmbio) |
| 5 | Análise e segmentação de clientes |
| 6 | Construção de dimensão de calendário |
| 7 | Modelo de previsão de demanda (Média Móvel — MAE) |
| 8 | Sistema de recomendação (similaridade de cosseno) |
| 9 | Análise exploratória complementar para material executivo |

## Stack

- Python 3 — pandas, numpy, matplotlib, seaborn, scikit-learn, duckdb
- JupyterLab

## Como Executar

```bash
# Instalar dependências
pip install pandas numpy matplotlib seaborn scikit-learn duckdb jupyterlab

# Clonar e rodar
git clone https://github.com/Marconiadsf/desafio-indicium-lighthouse
cd desafio-indicium-lighthouse
jupyter lab src/desafio_completo.ipynb
```

> O notebook usa caminhos relativos a partir de `src/`. Mantenha a estrutura de diretórios ao clonar.

---

**Autor:** Marconi Abou Dehn da Silva Filho  
**Data:** Março/2026
