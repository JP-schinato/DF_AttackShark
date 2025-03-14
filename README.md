# DF_AttackShark
Operações estatísticas e matemáticas no pandas

🔢 Operações básicas

sum() → Soma dos valores

mean() → Média (média aritmética)

median() → Mediana (valor central)

min() → Valor mínimo

max() → Valor máximo

std() → Desvio padrão

var() → Variância

📊 Operações acumuladas

cumsum() → Soma acumulada

cumprod() → Produto acumulado

cummin() → Mínimo acumulado

cummax() → Máximo acumulado

📈 Outras operações úteis

count() → Conta os valores não nulos

describe() → Estatísticas resumidas (média, min, max, etc.)

corr() → Correlação entre colunas numéricas

cov() → Covariância entre colunas numéricas
quantile(q) → Percentil (exemplo: df.quantile(0.25) para o primeiro quartil)

🎯 Operações com arredondamento

round(n) → Arredonda para n casas decimais

abs() → Valor absoluto

clip(lower, upper) → Limita os valores entre um mínimo e máximo

🔄 Transformações matemáticas

diff() → Diferença entre valores consecutivos

pct_change() → Variação percentual entre valores consecutivos

<-------------------x----------------------->
1. Criação e Carregamento de Dados

pd.DataFrame(data) → Cria um DataFrame

pd.Series(data) → Cria uma Series

pd.read_csv('arquivo.csv') → Lê um arquivo CSV

pd.read_excel('arquivo.xlsx') → Lê um arquivo Excel

pd.read_json('arquivo.json') → Lê um arquivo JSON

pd.read_sql(query, conexao) → Lê dados de um banco SQL

🔢 2. Operações Estatísticas e Matemáticas

df.sum() → Soma dos valores

df.mean() → Média

df.median() → Mediana

df.min() → Valor mínimo

df.max() → Valor máximo

df.std() → Desvio padrão

df.var() → Variância

df.cumsum() → Soma acumulada

df.cumprod() → Produto acumulado

df.count() → Contagem de valores não nulos

df.describe() → Estatísticas descritivas

📊 3. Manipulação de Dados

df.head(n) → Mostra as primeiras n linhas

df.tail(n) → Mostra as últimas n linhas

df.info() → Exibe informações do DataFrame

df.shape → Mostra (linhas, colunas)

df.columns → Lista os nomes das colunas

df.index → Exibe os índices

df.dtypes → Tipos de dados das colunas

df.rename(columns={'old': 'new'}) → Renomeia colunas

df.drop(columns=['coluna']) → Remove colunas

df.dropna() → Remove valores nulos

df.fillna(valor) → Preenche valores nulos

🔍 4. Filtros e Seleção de Dados

df['coluna'] → Seleciona uma coluna

df[['col1', 'col2']] → Seleciona múltiplas colunas

df.iloc[i, j] → Seleciona por índice de linha/coluna

df.loc[df['coluna'] > 10] → Filtra valores

df.query("coluna > 10") → Filtra com expressões

🔄 5. Transformação de Dados

df.apply(func) → Aplica uma função a colunas ou linhas

df.map(func) → Aplica uma função a uma Series

df.groupby('coluna').sum() → Agrupa por uma coluna

df.pivot(index, columns, values) → Cria tabelas dinâmicas

df.melt(id_vars, value_vars) → "Desempilha" o DataFrame

📌 6. Combinação e Junção de Dados

pd.concat([df1, df2]) → Concatena DataFrames

df.merge(df2, on='coluna', how='inner') → Faz joins (inner, left, right, outer)

df.append(df2) → Adiciona linhas

📅 7. Manipulação de Datas

pd.to_datetime(df['coluna']) → Converte para datetime

df['coluna'].dt.year → Extrai ano

df['coluna'].dt.month → Extrai mês

df['coluna'].dt.day → Extrai dia

df['coluna'].dt.weekday → Dia da semana

📊 8. Visualização de Dados

df.plot() → Gera gráficos básicos

df.hist() → Histograma

df.boxplot() → Boxplot

df.plot(kind='bar') → Gráfico de barras