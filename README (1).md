# ⚽ Football Players Analysis — Season 2024/25

## 🇧🇷 Português

### 📌 Sobre o projeto

Este projeto realiza uma análise exploratória de dados de jogadores de futebol referentes à temporada **2024/25**, utilizando Python, Pandas, Matplotlib e Seaborn.

O notebook utiliza dados de jogadores das **cinco principais ligas europeias** e analisa diferentes estatísticas individuais para identificar destaques ofensivos, defensivos e por posição.

Ao final, o projeto monta uma **Dream Team em uma formação 3-4-3**, selecionando jogadores com base em diferentes estatísticas.

### 🎯 Objetivos

- Carregar e selecionar dados relevantes dos jogadores;
- Analisar a distribuição de jogadores por liga;
- Analisar a distribuição de jogadores por posição;
- Identificar os 10 maiores goleadores;
- Identificar os 10 jogadores com mais assistências;
- Identificar os 10 jogadores com maior número de gols + assistências;
- Identificar os 10 jogadores com mais desarmes + interceptações;
- Identificar os 10 goleiros com mais defesas;
- Comparar estatísticas ofensivas e defensivas entre as ligas;
- Separar os jogadores por posição;
- Montar uma equipe 3-4-3 com base nas estatísticas analisadas.

### 📊 Estatísticas analisadas

| Estatística | Descrição |
|---|---|
| `Gls` | Gols |
| `Ast` | Assistências |
| `G+A` | Gols + Assistências |
| `Saves` | Defesas realizadas pelos goleiros |
| `Tkl+Int` | Desarmes + Interceptações |
| `KP` | Passes-chave |

### 🧩 Formação da Dream Team

A equipe final é construída no esquema **3-4-3**:

- **1 Goleiro:** maior número de defesas (`Saves`);
- **3 Defensores:** maior número de desarmes + interceptações (`Tkl+Int`);
- **4 Meio-campistas:** maior número de passes-chave (`KP`);
- **3 Atacantes:** maior número de gols + assistências (`G+A`).

### 🛠️ Tecnologias utilizadas

- **Python 3.12**
- **Pandas** — manipulação e análise dos dados;
- **Matplotlib** — criação de gráficos;
- **Seaborn** — visualização de dados;
- **Jupyter Notebook** — desenvolvimento e execução da análise.

### 📁 Estrutura esperada

```text
.
├── main.ipynb
├── players_data_light-2024_2025.csv
└── README.md
```

O arquivo CSV deve estar no mesmo diretório do notebook, pois o projeto o carrega diretamente com:

```python
pd.read_csv('players_data_light-2024_2025.csv', usecols=wanted_columns)
```

### ▶️ Como executar

1. Instale o Python 3.12 ou uma versão compatível.
2. Instale as dependências:

```bash
pip install pandas matplotlib seaborn jupyter
```

3. Coloque `main.ipynb` e `players_data_light-2024_2025.csv` na mesma pasta.
4. Inicie o Jupyter Notebook:

```bash
jupyter notebook
```

5. Abra `main.ipynb`.
6. Execute as células em ordem.

### 📈 Visualizações

O notebook gera gráficos de barras para:

- Top 10 goleadores;
- Top 10 assistentes;
- Top 10 jogadores em G+A;
- Top 10 jogadores em Tkl+Int;
- Top 10 goleiros em número de defesas.

Além dos gráficos, são realizadas agregações por liga para comparar médias de estatísticas ofensivas e defensivas.

### ⚠️ Observações

A seleção dos jogadores da Dream Team é baseada exclusivamente nas métricas utilizadas no notebook. Portanto, a equipe não representa necessariamente uma avaliação completa da qualidade dos jogadores, já que outros fatores e estatísticas não são considerados.

---

# ⚽ Football Players Analysis — 2024/25 Season

## 🇺🇸 English

### 📌 About the project

This project performs an exploratory data analysis of football players from the **2024/25 season**, using Python, Pandas, Matplotlib, and Seaborn.

The notebook uses player data from the **top five European leagues** and analyzes different individual statistics to identify offensive and defensive highlights, as well as players by position.

At the end, the project builds a **Dream Team using a 3-4-3 formation**, selecting players according to different statistical criteria.

### 🎯 Objectives

- Load and select relevant player data;
- Analyze the distribution of players by league;
- Analyze the distribution of players by position;
- Identify the top 10 goalscorers;
- Identify the top 10 players by assists;
- Identify the top 10 players by goals + assists;
- Identify the top 10 players by tackles + interceptions;
- Identify the top 10 goalkeepers by saves;
- Compare offensive and defensive statistics between leagues;
- Group players by position;
- Build a 3-4-3 Dream Team based on the analyzed statistics.

### 📊 Analyzed statistics

| Statistic | Description |
|---|---|
| `Gls` | Goals |
| `Ast` | Assists |
| `G+A` | Goals + Assists |
| `Saves` | Saves made by goalkeepers |
| `Tkl+Int` | Tackles + Interceptions |
| `KP` | Key Passes |

### 🧩 Dream Team formation

The final team is built using a **3-4-3 formation**:

- **1 Goalkeeper:** highest number of saves (`Saves`);
- **3 Defenders:** highest number of tackles + interceptions (`Tkl+Int`);
- **4 Midfielders:** highest number of key passes (`KP`);
- **3 Forwards:** highest number of goals + assists (`G+A`).

### 🛠️ Technologies

- **Python 3.12**
- **Pandas** — data manipulation and analysis;
- **Matplotlib** — data visualization;
- **Seaborn** — statistical visualization;
- **Jupyter Notebook** — development and execution of the analysis.

### 📁 Expected structure

```text
.
├── main.ipynb
├── players_data_light-2024_2025.csv
└── README.md
```

The CSV file must be located in the same directory as the notebook because it is loaded directly with:

```python
pd.read_csv('players_data_light-2024_2025.csv', usecols=wanted_columns)
```

### ▶️ How to run

1. Install Python 3.12 or a compatible version.
2. Install the required dependencies:

```bash
pip install pandas matplotlib seaborn jupyter
```

3. Place `main.ipynb` and `players_data_light-2024_2025.csv` in the same directory.
4. Start Jupyter Notebook:

```bash
jupyter notebook
```

5. Open `main.ipynb`.
6. Run the cells in order.

### 📈 Visualizations

The notebook generates bar charts for:

- Top 10 goalscorers;
- Top 10 assist providers;
- Top 10 players by G+A;
- Top 10 players by Tkl+Int;
- Top 10 goalkeepers by saves.

The project also performs league-level aggregations to compare average offensive and defensive statistics.

### ⚠️ Notes

The Dream Team selection is based exclusively on the metrics used in the notebook. Therefore, it does not represent a complete assessment of player quality, since other statistics and factors are not considered.
