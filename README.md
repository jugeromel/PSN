# Análise de Dados PNS - Fatores Associados à Saúde Mental e Alimentação

Este repositório contém os códigos e as análises realizadas a partir dos dados da **Pesquisa Nacional de Saúde (PNS)**, com o objetivo de estudar os **fatores associados à saúde mental**, como **depressão** e **outros diagnósticos de doenças mentais**, bem como o impacto dos hábitos alimentares e dietas nas condições de saúde. A análise foi realizada utilizando **STATA** para manipulação de dados, modelagem estatística e visualização de resultados.

## Estrutura do Repositório

O repositório está organizado da seguinte forma:


/pns_data ├── pns_2019.dta # Dados da PNS 2019 tratados ├── pns_health_data.dta 
# Dados sobre saúde mental e alimentação ├── pns_cleaned.dta 
# Dados limpos e prontos para análise /stata_scripts ├── 01_eda_pns.do 
# Código STATA para análise exploratória dos dados da PNS ├── 02_regressao_pns.do 
# Código STATA para análise de regressão sobre fatores de saúde mental ├── 03_saude_mental.dta 
# Código STATA para análise da relação entre saúde mental e alimentação ├── 04_dummy_variables.dta 
# Código STATA para criação de variáveis ​​dummy /resultados ├── resultados_logit_depressao.csv 
# Resultados do modelo Logit para análise de depressão ├── resultados_logit_outro_diagnostico.csv 
# Resultados do modelo Logit para outros diagnósticos ├── figuras 
# Gráficos e visualizações geradas durante a análise ├── descritivas_pns.xlsx # Tabelas de estatísticas descritivas exportadas para Excel


## Descrição

### Objetivo

Este projeto visa explorar dados da **PNS 2019** para entender as relações entre características socioeconômicas, comportamentais e alimentares com a **saúde mental** dos indivíduos. Em particular, estamos investigando a prevalência de **depressão**, **outros diagnósticos de doenças mentais** e as influências de uma **dieta saudável e não saudável**.

### Principais variáveis analisadas:

- **Saúde mental**: Identificação de indivíduos com diagnóstico de **depressão** ou outros transtornos mentais.
- **Hábitos alimentares**: Variáveis que indicam se o indivíduo segue uma dieta saudável ou não saudável, como consumo de **feijão**, **verduras**, **carne vermelha**, **frango**, **peixe**, entre outros.
- **Variáveis sociodemográficas**: Como **idade**, **sexo**, **renda**, **localização (urbano ou rural)**, e **raça**.
- **Análises realizadas**:
  - Modelos de **regressão logística (logit)** para avaliar os fatores associados à **depressão** e **outros diagnósticos**.
  - Análise de variáveis **dummies** para características como **sexo**, **renda**, e **localização**.

### Scripts STATA

1. **`01_eda_pns.do`**: Realiza uma análise exploratória dos dados da PNS, incluindo a limpeza de dados e a criação de variáveis dummies para as categorias de interesse.
2. **`02_regressao_pns.do`**: Executa modelos de regressão para avaliar os fatores associados à **depressão** e outros **diagnósticos de doenças mentais**.
3. **`03_saude_mental.dta`**: Código para a análise dos hábitos alimentares em relação à saúde mental dos indivíduos.
4. **`04_dummy_variables.dta`**: Gera variáveis dummies para facilitar a análise de grupos categóricos.

### Análises e Resultados

Os resultados de regressões logísticas e estatísticas descritivas são exportados para **arquivos CSV** e **Excel**, incluindo estatísticas como **média de renda** por grupo de saúde mental, e distribuições de diagnóstico por **sexo** e **localização geográfica**.

## Como rodar os códigos

1. **Carregar os dados**: Execute o código `use "C:\caminho\para\pns_data.dta", clear` para carregar o arquivo de dados no STATA.
2. **Executar as análises**: Rode os scripts **STATA** para realizar análises descritivas, regressões e exportação de resultados.
3. **Interpretação dos resultados**: Os resultados dos modelos logit serão gerados nos arquivos `resultados_logit_depressao.csv`, `resultados_logit_outro_diagnostico.csv`, entre outros.

## Contribuições

Se você quiser contribuir com este projeto, fique à vontade para fazer **fork**, **criar issues** e enviar **pull requests**. Agradecemos qualquer feedback e colaboração!

## Licença

Este projeto está licenciado sob a **Licença MIT** - veja o arquivo [LICENSE](LICENSE) para mais detalhes.

**Contato:**
- Nome: Juliana Geromel
- Email: geromeljuliana@gmail.com
- LinkedIn: (https://www.linkedin.com/in/juliana-geromel/)

