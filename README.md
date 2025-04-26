# Projeto da disciplina de análise de dados
 
- Membros da equipe: Yves Pereira e Thiago Raimundo
- Objetivo do projeto: Analisar se o aumento do bolsa família influencia 
na diminuição do abandono escolar no Brasil entre os anos de 2012 e 2021


## Objetivo
Investigar a relação entre o programa Bolsa Família (BF) e as taxas de abandono escolar no **Ensino Fundamental (EF)** e **Ensino Médio (EM)**, controlando por variáveis socioeconômicas e educacionais.

## Variáveis Utilizadas
### **Variável Dependente (Alvo)**:
- `Abandono_EF`: Taxa de abandono escolar no Ensino Fundamental  
- `Abandono_EM`: Taxa de abandono escolar no Ensino Médio  

### **Variáveis Independentes (Explicativas)**:
#### **1. Bolsa Família**:
- `Valor_medio_BF`: Valor médio mensal recebido por família (R$)  
- `QTD_FAMILIAS_BF`: Número de famílias beneficiárias  

#### **2. Indicadores Educacionais**:
- `IDHM Educação`: Índice de Desenvolvimento Humano Municipal (dimensão educação)  
- `Índice de Atkinson Educação`: Medida de desigualdade educacional  

#### **3. Indicadores Econômicos**:
- `Taxa de Desocupação`: % da população economicamente ativa desempregada  
- `Taxa de Participação`: % da população em idade ativa no mercado de trabalho  
- `Nível de Ocupação`: % da população economicamente ativa empregada  
- `Índice de Gini`: Medida de desigualdade de renda (0 a 1)  
- `Índice de Atkinson Renda`: Desigualdade de renda (sensível a extremos)  

### Como estão distribuídos os dados nas pastas:
- `alunos_matriculados`: dados absolutos com a quantidade de alunos matriculados em cada estado  
- `rendimento_escolar`: dados com a taxa de abandono por estado com localização abrangendo áreas rurais e urbanas e rede total incluindo escolas públicas e privadas 
- `total_abandono_alunos_estados`: dados provenientes da multiplicação de alunos matriculados e rendimento escolar 
- `dadosUsadosParaMerge`: dados absolutos e taxas que foram usados para acrescentar em um dataframe e assim poder fazer a análise dos dados
- `dados_medios`: dados com média, dos anos de 2012 até 2021, que foram utilizados para gerar mapas interativos no geobr
- `conversãoDados`: onde está localizado todo o código para mesclar, somar, multplicar dados de planilhas e salvar em outras
- `analises_regressão`:  foi realidos os testes de correlação entre as variaveis usadas, além disso tambem foram geradas tabelas de correlação e gráficos de dispersão de todos os anos. Foi realizado também a mesclagem dos dados que foram usados para o modelo OLS e por fim realizando o teste. No final há a inclusão do mapa com os dados da pasta **dados_medios** para gerar o mapa de calor do Brasil


### Arquivos:
- `analise_robusta.csv`: arquivo com todos os dados utilizados 
- `OBS.`: indicadores tabela é utilizado para fazer a taxa de desocupação, dado esse que está em **dadosUsadosParaMerge**
