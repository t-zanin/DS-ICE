(Portuguese version below)

# Game Sales Analysis - Ice Project

## Overview

This project was developed for a data analysis learning sprint. The goal is to analyze historical video game sales data from the Ice online store, which sells games globally, to identify patterns that determine a game's success.

Based on sales data, user and critic ratings, genres, platforms, and ESRB classifications, the project aims to generate insights for planning effective advertising campaigns for 2017, using data up to 2016.

Key steps include:

- **Data preparation**: Handling missing values, converting data types, and creating a total sales column.
- **Exploratory analysis**: Examining release distribution, sales by platform, genres, and the impact of ratings.
- **Regional profile**: Identifying top platforms and genres by region (North America, Europe, and Japan).
- **Hypothesis testing**: Checking for differences in user ratings between platforms (Xbox One and PC) and genres (Action and Sports).

---

## Prerequisites

To run the project, you will need the following tools and libraries:

- Python 3.8+
- Python libraries:
  - pandas
  - numpy
  - matplotlib
  - scipy
- Jupyter Notebook (to run the provided code)
- Data file: `games.csv` (available at `/games.csv`)

---

## How to Run

1. Open the `analysis.ipynb` file in a Jupyter Notebook environment.
2. Make sure the `games.csv` file is in the correct directory.
3. Run all the cells in the notebook to perform the full analysis, including:
   - Loading and preparing the data.
   - Generating charts (bar, line, boxplots, and scatter).
   - Performing statistical calculations and hypothesis tests.

---

## Project Structure

The project is organized into a Jupyter Notebook (`analysis.ipynb`) with the following sections:

### Initial Data Exploration

- Load the `games.csv` file.
- Perform initial inspection to identify data issues.

### Data Preparation

- Rename columns to lowercase.
- Convert `year_of_release` to integer and `user_score` to float, treating `'TBD'` values as NaN.
- Fill missing values in `rating` with `'N/A'`.
- Create a `total_sales` column by summing regional sales.

### Data Analysis

- Distribution of game releases per year, peaking in 2008–2009.
- Platform sales highlighting PS2, Xbox 360, and PS3 as historical leaders, and PS4 and Xbox One in 2016.
- Average platform lifecycle (7.6 years) and time to peak sales (3.9 years).
- Sales analysis by genre, with Platform, Shooter, and RPG leading.
- Weak correlation (0.23) between critic scores and sales on PS4.

### Regional Profile

- **North America**: Xbox 360 dominates, followed by PS2 and Wii. Action and shooter games are popular.
- **Europe**: Balanced presence of PS3, PS2, and Xbox 360, with a focus on racing games.
- **Japan**: Preference for handheld consoles (DS, PSP) and genres like RPG and Platform.

### Hypothesis Testing

- **Hypothesis 1**: Average user ratings for Xbox One and PC are different (p-value < 0.05).
- **Hypothesis 2**: Average ratings for Action and Sports genres are different (p-value < 0.05).

---

## Key Findings

- **Platform Lifecycle**: On average, platforms last 7.6 years, with peak sales occurring after ~3.9 years.
- **Market Trends**: PS4 and Xbox One led sales in 2016, while older platforms (PS3, Xbox 360, Wii) lost relevance.
- **Top Genres**: Platform, Shooter, and RPG genres have the highest average sales, with notable regional differences (RPGs dominate in Japan, while Action and Shooter lead in the West).
- **Ratings Impact**: Critic ratings have a weak positive correlation with sales on PS4, suggesting other influential factors.
- **Regional Preferences**:
  - North America: Focus on Xbox and action games.
  - Europe: Balanced interest between Sony and Microsoft, with popularity in racing games.
  - Japan: Preference for handheld consoles and RPGs.
- **ESRB Ratings**: Games rated E (Everyone) and T (Teen) dominate global sales, though Japan uses its own rating system.

---

## Hypothesis Tests

- **Hypothesis 1**: Null hypothesis rejected (H₀: average ratings for Xbox One and PC are equal). Significant difference found (p-value < 0.05).
- **Hypothesis 2**: Null hypothesis rejected (H₀: average ratings for Action and Sports genres are equal). Significant difference found (p-value < 0.05).

---

## Final Conclusion

The project revealed that the video game market is dynamic, with clear technology replacement cycles, where newer platforms like PS4 and Xbox One dominate as older ones fade out.

Genres and preferences vary significantly by region, with RPGs more popular in Japan and Action and Shooter games prevailing in the West. Critic reviews have limited influence on sales, suggesting other factors like marketing and nostalgia may be more impactful.

Statistical analysis confirmed differences in user ratings between platforms and genres, providing valuable insights for advertising strategies in 2017.

---

## How to Contribute

1. Fork the repository.
2. Create a new branch for your feature:
3. Commit your changes:(git commit -m "Add new analysis")
4. Push to the branch: (git push origin feature/new-analysis)

---

## License

This project is licensed under the MIT License.

__________________________________________________________________
__________________________________________________________________
__________________________________________________________________
__________________________________________________________________

Versão em português

# Análise de Vendas de Jogos - Projeto Ice

## Visão Geral

Este projeto foi desenvolvido para análise de dados. O objetivo é analisar dados históricos de vendas de jogos da loja online Ice, que comercializa videogames globalmente, para identificar padrões que determinam o sucesso de um jogo.

Com base em dados de vendas, avaliações de usuários e críticos, gêneros, plataformas e classificações ESRB, o projeto busca insights para planejar campanhas publicitárias eficazes para 2017, utilizando dados até 2016.

As principais etapas incluem:

- **Preparação dos dados**: Tratamento de valores ausentes, conversão de tipos de dados e criação de uma coluna de vendas totais.
- **Análise exploratória**: Estudo da distribuição de lançamentos, vendas por plataforma, gêneros e impacto das avaliações.
- **Perfil regional**: Identificação das principais plataformas e gêneros por região (América do Norte, Europa e Japão).
- **Teste de hipóteses**: Verificação de diferenças nas avaliações de usuários entre plataformas (Xbox One e PC) e gêneros (Action e Sports).

---

## Pré-requisitos

Para executar o projeto, você precisará das seguintes ferramentas e bibliotecas:

- Python 3.8+
- Bibliotecas Python:
  - pandas
  - numpy
  - matplotlib
  - scipy
- Jupyter Notebook (para executar o código fornecido)
- Arquivo de dados: `games.csv` (disponível em `/games.csv`)

## Como Executar

1. Abra o arquivo `analysis.ipynb` em um ambiente Jupyter Notebook.
2. Certifique-se de que o arquivo `games.csv` está no diretório correto.
3. Execute todas as células do notebook para realizar a análise completa, incluindo:
   - Carregamento e preparação dos dados.
   - Geração de gráficos (barras, linhas, boxplots e dispersão).
   - Cálculos estatísticos e testes de hipóteses.

---

## Estrutura do Projeto

O projeto está organizado em um Jupyter Notebook (`analysis.ipynb`) com as seguintes seções:

### Exploração Inicial dos Dados

- Carregamento do arquivo `games.csv`.
- Inspeção inicial para identificar problemas nos dados.

### Preparação dos Dados

- Renomeação de colunas para letras minúsculas.
- Conversão de `year_of_release` para inteiro e `user_score` para float, tratando valores `'TBD'` como NaN.
- Preenchimento de valores ausentes em `rating` com `'N/A'`.
- Criação da coluna `total_sales` somando vendas regionais.

### Análise de Dados

- Distribuição de lançamentos por ano, com pico em 2008–2009.
- Vendas por plataforma, destacando PS2, Xbox 360 e PS3 como líderes históricas, e PS4 e Xbox One em 2016.
- Ciclo de vida médio das plataformas (7,6 anos) e tempo para atingir o pico de vendas (3,9 anos).
- Análise de vendas por gênero, com Platform, Shooter e RPG liderando.
- Correlação fraca (0,23) entre pontuações críticas e vendas no PS4.

### Perfil Regional

- **América do Norte**: Predominância do Xbox 360, seguido por PS2 e Wii. Gêneros de ação e shooters são populares.
- **Europa**: Equilíbrio entre PS3, PS2 e Xbox 360, com destaque para jogos de corrida.
- **Japão**: Preferência por consoles portáteis (DS, PS) e gêneros como RPG e Platform.

### Teste de Hipóteses

- **Hipótese 1**: As classificações médias de usuários para Xbox One e PC são diferentes (p-valor < 0,05).
- **Hipótese 2**: As classificações médias para gêneros Action e Sports são diferentes (p-valor < 0,05).

---

## Principais Resultados

- **Ciclo de Vida das Plataformas**: Em média, plataformas têm uma vida útil de 7,6 anos, com pico de vendas em ~3,9 anos.
- **Tendências de Mercado**: PS4 e Xbox One dominaram as vendas em 2016, enquanto plataformas mais antigas (PS3, Xbox 360, Wii) perderam relevância.
- **Gêneros Lucrativos**: Platform, Shooter e RPG lideram em vendas médias, com diferenças regionais significativas (RPGs dominam no Japão, enquanto ação e shooters prevalecem no Ocidente).
- **Impacto das Avaliações**: Avaliações críticas têm uma correlação positiva fraca com vendas no PS4, sugerindo outros fatores influentes.
- **Preferências Regionais**:
  - América do Norte: Foco em Xbox e jogos de ação.
  - Europa: Equilíbrio entre Sony e Microsoft, com interesse em jogos de corrida.
  - Japão: Preferência por consoles portáteis e RPGs.
- **Classificações ESRB**: Jogos classificados como E (Everyone) e T (Teen) dominam vendas globalmente, mas o Japão utiliza sistemas próprios de classificação.

---

## Testes de Hipóteses

- **Hipótese 1**: Rejeitada a hipótese nula (H₀: classificações médias de Xbox One e PC são iguais). Há diferença significativa (p-valor < 0,05).
- **Hipótese 2**: Rejeitada a hipótese nula (H₀: classificações médias de Action e Sports são iguais). Há diferença significativa (p-valor < 0,05).

---

## Conclusão Geral

O projeto revelou que o mercado de videogames é dinâmico, com ciclos de substituição tecnológica claros, onde novas plataformas como PS4 e Xbox One dominam à medida que as antigas desaparecem.

Gêneros e preferências variam significativamente por região, com RPGs sendo mais populares no Japão e jogos de ação e shooters no Ocidente. As avaliações críticas têm impacto limitado nas vendas, indicando a influência de outros fatores como marketing e nostalgia.

As análises estatísticas confirmaram diferenças nas avaliações de usuários entre plataformas e gêneros, fornecendo insights valiosos para campanhas publicitárias em 2017.

---

## Como Contribuir

1. Faça um fork do repositório.
2. Crie uma branch para sua feature:('git checkout -b feature/nova-analise').
3. Commit suas alterações ('git commit -m 'Adiciona nova análise'').
4. Push para a branch ('git push origin feature/nova-analise').

---

## Licença

Este projeto está licenciado sob a MIT License.