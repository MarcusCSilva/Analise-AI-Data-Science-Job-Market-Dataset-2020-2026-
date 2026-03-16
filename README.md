#  Análise de Dados: Mercado de Trabalho em AI & Data Science (2020–2026)

##  Sobre o Projeto
O mercado de Inteligência Artificial e Ciência de Dados é um dos que mais cresce e se transforma no mundo. Este projeto é uma Análise Exploratória de Dados (EDA) baseada no dataset "AI & Data Science Job Market (2020–2026)", com o objetivo de entender o cenário de contratações, exigências técnicas e remunerações da área.

O objetivo principal foi realizar a limpeza da base de dados, criar novas categorizações de senioridade e extrair métricas de negócio focadas em médias salariais, modelos de trabalho (remoto/híbrido/presencial) e as habilidades (skills) mais requisitadas por setor.

##  Ferramentas Utilizadas
- **Linguagem:** Python
- **Bibliotecas:** Pandas, NumPy, Matplotlib / Seaborn (para visualização)
- **Ambiente:** Jupyter Notebook

##  Tratamento e Limpeza de Dados (Data Cleaning)
A base de dados passou por um rigoroso processo de auditoria e limpeza para garantir que os cálculos estatísticos fossem precisos. As principais etapas foram:
1. **Correção de Tipos de Dados (Casting):** Identificação e conversão da coluna de salários (`Salary`) para o tipo numérico (`float`), viabilizando as operações matemáticas.
2. **Tratamento de Anomalias (Outliers):** Utilização de gráficos de dispersão (Boxplot) para identificar salários completamente fora do padrão. Esses registros foram analisados e removidos para não distorcer as médias salariais.
   <img width="608" height="422" alt="Outlier_boxplot" src="https://github.com/user-attachments/assets/e8a4ad0c-8eff-407b-9fce-027bc4117360" />
4. **Validação de Integridade:** Verificação e remoção de dados duplicados, além da confirmação de que colunas geográficas fundamentais (como `Country`) não possuíam valores ausentes (nulos).
5. **Engenharia de Atributos (Feature Engineering):** Criação de uma nova tabela e categorização dos níveis de experiência dos profissionais, padronizando-os em três grandes grupos: **Júnior, Pleno e Sênior**.

##  Principais Questionamentos de Negócio
Durante a Análise Exploratória, busquei responder às seguintes perguntas:
1. Qual é a média salarial dos profissionais dividida por setor de atuação?
2. Como o modelo de trabalho (remoto, híbrido ou presencial) impacta a remuneração final?
3. Quais são as linguagens de programação e *skills* mais requisitadas dentro de cada setor?
4. Como os salários se distribuem entre as diferentes senioridades (Júnior, Pleno, Sênior)?

##  Resultados e Insights

### 1. Média Salarial por Setor e Senioridade
Os cargos com as maiores remunerações são **AI Engineer**, **Machine Learning Engineer** e **Data Scientist**. Essas posições apresentam a maior valorização salarial conforme o avanço da senioridade, impulsionadas pela alta demanda por formações complexas, como *Deep Learning* e *Cloud Computing*. A análise comprovou que o teto salarial do profissional está diretamente ligado ao seu nível de especialização técnica e ao nicho de atuação.

### 2. Impacto do Modelo de Trabalho
O modelo **Remoto** apresentou a maior média salarial do mercado, enquanto o formato **Presencial** registrou a mais baixa. Essa diferença sugere que a redução de custos operacionais das empresas (como infraestrutura física e auxílios de deslocamento) permite o repasse desses valores para a remuneração direta do colaborador, otimizando o orçamento corporativo.

### 3. Skills e Linguagens Dominantes
A análise de ferramentas revelou um perfil de especialização claro para cada cargo:
- **Business Analyst:** Forte presença de ferramentas *Cloud*.
- **AI Engineer:** Domínio absoluto em *Deep Learning*.
- **Machine Learning Engineer:** Foco expressivo em ferramentas de *Machine Learning* e *Cloud*.
- **Data Analyst:** Alta demanda e consolidação no uso de *SQL* e *Python*.
- **Data Scientist:** Combinação técnica focada em *Machine Learning* e *SQL*.
- **Data Engineer:** Forte exigência em infraestrutura *Cloud* e *Python*.

