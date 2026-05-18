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

| **Fase 2** | Limpeza e Preparação do Dataset | Felipe | Concluído |

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

---

## Insights do Projeto Integrador: Catálogo Netflix
**1. Parte: Henrique (Análise de Perfil de Público - Rating)**

Esta análise foca na segmentação demográfica do catálogo com base nas classificações indicativas.

* **Dominância do Público Adulto:** O catálogo apresenta uma concentração massiva em produções TV-MA (mais de 3.200 títulos), o que posiciona a Netflix estrategicamente como uma plataforma voltada para o consumo de jovens adultos e adultos.

* **Distribuição por Faixa Etária:** A segunda maior categoria é a TV-14, indicando que a maior parte do esforço de licenciamento e produção original visa conteúdos com temáticas mais complexas ou maduras.

* **Gap de Conteúdo Infantil:** Existe uma queda acentuada no volume de títulos para as classificações TV-Y, TV-G e G. Estrategicamente, isso sugere que o perfil de público da plataforma é menos focado em nichos estritamente infantis em comparação ao volume total de títulos disponíveis.

**2. Parte: Mariucha (Tendências e Distribuição de Duração)**

A Mariucha explorou a evolução temporal e a densidade da duração das obras.

* **Histórico de Longa Duração:** Identificou-se um período de produções extensas por volta dos anos 60, com médias que chegavam a 200 minutos.

* **Padronização Contemporânea:** Atualmente, há uma convergência para o formato de 100 minutos, refletindo uma adaptação às janelas de atenção do espectador moderno.

* **Volume de Produção:** O histograma confirma que a grande massa do catálogo está situada entre 80 e 120 minutos, definindo o padrão de "filme comercial" da plataforma.

**3. Parte: Andrey (Volumetria e Retenção de Séries)**

Esta análise foca no ciclo de vida das séries e na capacidade de retenção de títulos a longo prazo dentro da plataforma.

* **Alto Índice de Descontinuação:** O catálogo apresenta uma concentração massiva de séries com "Temporada Única", representando 67.0% do total (1.793 títulos). Isso evidencia uma estratégia de ampla experimentação de mercado, onde muitos títulos são lançados para testar a recepção do público.

* **Funil de Renovação Estrito:** Apenas 33.0% das produções alcançam o status de "Séries Longevas" (883 títulos), sobrevivendo à barreira da primeira temporada. Estrategicamente, manter produções por múltiplos anos exige investimentos crescentes, justificando o rigor na seleção para renovações.

* **Modelo Baseado em Novidades:** A distribuição confirma que o modelo de negócios da Netflix prioriza a rotatividade constante e o hype de novos lançamentos em vez da manutenção prolongada de histórias extensas.
