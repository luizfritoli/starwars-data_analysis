# *Análise exploratória com dados de Star Wars*

Neste repositório, estão sendo feitos tratamento e análise da tabela
"starwars", com base nos dados fornecidos pela biblioteca `Tidyverse`. 

## *Estrutura*

- `data/raw`: Dados originais.
- `data/clean`: Dados após tratamento (limpos).
- `scripts/cleaning.Rmd`: Script responsável pelo filtro inicial e limpeza dos dados.
- `scripts/analysis.Rmd`: Script responsável pela análise dos dados usando gráficos e tabelas.

## *Análises e considerações*

1. **Correlação entre altura e massa**

   Existe uma correlação significativa entre os dados "altura" e "massa". Depois de analisar
   a tendência de correlação de forma simples usando a biblioteca `Ggcorrplot`, primeiramente
   sem filtros, o resultado do cálculo foi 0.13 (baixa correlação).

   No entanto, após filtrar o único outlier (massa < 1000), apresentou uma correlação 
   considerável de 0.75.
  
   Então, o filtro também foi realizado no momento de criação do gráfico foi confirmado via 
   gráfico de dispersão que a tendência é real (não obrigatória): quanto maior for o sujeito,
   a massa tende a aumentar da mesma forma.
  