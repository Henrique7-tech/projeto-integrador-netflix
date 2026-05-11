#  Análise Estratégica do Catálogo Netflix

Base de dados: https://www.kaggle.com/datasets/shivamb/netflix-shows/data

O objetivo é realizar uma análise exploratória de dados (EDA) utilizando para entender o perfil de conteúdo e a estratégia de atualização da plataforma Netflix.

---

##  Objetivos da Análise

Buscamos responder perguntas estratégicas sobre o catálogo:

1.  **Janela de Lançamento:** Qual o tempo médio entre o lançamento original de uma obra e sua chegada ao catálogo?

2.  **Ciclo de Vida das Séries:** A Netflix foca em séries de longa duração ou em produções de temporada única?

3.  **Perfil de Audiência:** O catálogo é majoritariamente voltado para qual faixa etária (Rating)?

4.  **Padrão de Duração:** Qual a duração média dos filmes e como isso variou nos últimos anos?

---

## Estrutura de Pastas

**dados/raw/**: Contém o arquivo original netflix_titles.csv

**dados/processed/**: Contém o arquivo limpo netflix_clean.csv

**notebooks/**: Contém o código Python de tratamento de dados

---

##  Equipe

* **Felipe Yudi Higashi (Engenharia):** Limpeza de dados, tratamento de valores nulos e criação de colunas temporais.

* **Mariucha Jobim (Análise de Filmes):** Estudo de métricas de duração, médias, medianas e tendências de tempo dos filmes.

* **Andrey de Souza Sezário (Análise de Séries):** Estudo de volumetria de temporadas e taxa de retenção/renovação de séries.

* **Henrique Nascimento de Souza (Qualidade e Documentação):** Análise de perfil de público (Rating), consolidação dos insights e organização do repositório.

---

##  Cronograma de Execução

| **Fase 1** | Estruturação do GitHub e README | Todos |  Concluído |

| **Fase 2** | Limpeza e Preparação do Dataset | Felipe | Em espera |

| **Fase 3** | Análise Técnica e Gráficos | Mariucha e Andrey | Em espera |

| **Fase 4** | Consolidação de Insights e Entrega | Henrique | Em espera |

---

## Planejamento de Transformações 

Para que as análises sejam precisas, realizaremos as seguintes manipulações:

* **Conversão de Datas:** Transformar a coluna date_added para o formato de data (YYYY-MM-DD).

* **Cálculo de Janela:** Criar uma nova métrica subtraindo o release_year do ano de adição no catálogo.

* **Tratamento de Texto:** Limpar a coluna duration para separar valores numéricos de unidades (minutos vs temporadas).

---

## Planejamento de Visualizações (Dashboard)

Pretendemos apresentar os seguintes indicadores:

* **Gráfico de Barras:** Distribuição de títulos por rating (Público-alvo).

* **Gráfico de Linhas:** Evolução da duração média dos filmes ao longo dos anos.

* **Histograma:** Frequência do tempo de espera (Janela de Lançamento).

* **Gráfico de Rosca:** Proporção entre produções de temporada única e séries longevas.
