# Análise de Dados SINASC - Efeitos do Zika na Taxa de Nascimentos

Este repositório contém os códigos e as análises realizadas a partir dos dados do **Sistema de Informações sobre Nascidos Vivos (SINASC)**, com o objetivo de estudar os **efeitos do Zika vírus na taxa de nascimentos** no Brasil. O projeto inclui manipulação de dados, modelagem estatística e visualização de resultados.

## Estrutura do Repositório

O repositório está organizado da seguinte forma:
/sinasc_data ├── sinasc_2015.dta # Dados de nascimentos em 2015 ├── sinasc_2016.dta 
# Dados de nascimentos em 2016 ├── sinasc_cleaned.dta 
# Dados tratados e preparados para análise ├── sinasc_zika_impact.dta 
# Dados de impacto do Zika na taxa de nascimentos /notebooks ├── 01_eda_sinasc.ipynb 
# Análise exploratória dos dados SINASC ├── 02_regressao_sinasc.ipynb 
# Modelagem de regressão sobre os dados SINASC ├── 03_impacto_zika.ipynb 
# Análise do impacto do Zika na taxa de nascimentos /results ├── resultados_logit.csv 
# Resultados do modelo Logit para a análise de nascimentos ├── resultados_regressao.csv 
# Resultados da regressão sobre a taxa de nascimentos ├── figuras 
# Gráficos e visualizações geradas durante a análise


## Descrição dos Arquivos

### Dados

- **sinasc_2015.dta**: Contém os dados de nascimentos no Brasil referentes ao ano de 2015.
- **sinasc_2016.dta**: Contém os dados de nascimentos no Brasil referentes ao ano de 2016.
- **sinasc_cleaned.dta**: Dados tratados e limpos, com remoção de valores ausentes e variáveis irrelevantes.
- **sinasc_zika_impact.dta**: Dados relacionados ao impacto do Zika vírus sobre a taxa de nascimentos, com indicadores de áreas afetadas pela epidemia.

### Notebooks

- **01_eda_sinasc.ipynb**: Realiza uma análise exploratória de dados (EDA) sobre os dados SINASC, incluindo visualizações como histogramas, boxplots e tabelas descritivas.
- **02_regressao_sinasc.ipynb**: Contém o código para a modelagem de regressão, avaliando o impacto de variáveis como idade da mãe, raça e local de nascimento na taxa de nascimentos.
- **03_impacto_zika.ipynb**: Foca especificamente na análise do impacto do Zika vírus nas taxas de nascimentos, incluindo regressões e modelos para entender a correlação entre a epidemia e os resultados de nascimento.

### Resultados

- **resultados_logit.csv**: Arquivo contendo os resultados do modelo de regressão logística (logit) que estima a probabilidade de nascimentos com complicações associadas ao Zika.
- **resultados_regressao.csv**: Resultados de regressões múltiplas, considerando as variáveis explicativas e a taxa de nascimentos.
- **figuras**: Pasta com gráficos e visualizações geradas durante as análises, incluindo gráficos de dispersão, regressões e boxplots.

## Requisitos

Para executar os códigos e realizar as análises, você precisa ter os seguintes pacotes instalados:

- **Python** (versão 3.6 ou superior)
  - `pandas`
  - `numpy`
  - `matplotlib`
  - `seaborn`
  - `statsmodels`
  - `scikit-learn`
  - `jupyter`
- **STATA** (para manipulação de dados `.dta` e execução de scripts STATA)
- **R** (caso você tenha scripts adicionais de análise estatística)

## Como Executar os Códigos

1. **Baixe os dados**: Carregue as bases de dados SINASC (disponíveis na pasta `sinasc_data`).
2. **Execute a Análise Exploratória (EDA)**: Abra o notebook `01_eda_sinasc.ipynb` e execute as células para começar a análise exploratória.
3. **Rodar Modelos de Regressão**: Acesse o notebook `02_regressao_sinasc.ipynb` para aplicar modelos de regressão e avaliar as variáveis que impactam a taxa de nascimentos.
4. **Analisar Impacto do Zika**: Abra o notebook `03_impacto_zika.ipynb` para entender como a epidemia de Zika afetou a taxa de nascimentos, com base nos dados regionais.
5. **Revisar Resultados**: Os resultados das análises e modelos estarão na pasta `/results`, onde você pode visualizar as tabelas e gráficos gerados.

## Contribuições

Contribuições para melhorar o código e os resultados são bem-vindas! Se você deseja contribuir, siga as etapas abaixo:

1. Faça um fork deste repositório.
2. Crie uma nova branch (`git checkout -b minha-nova-branch`).
3. Realize as alterações necessárias e faça um commit (`git commit -m 'Adicionando novas análises'`).
4. Envie a sua branch para o repositório remoto (`git push origin minha-nova-branch`).
5. Abra um pull request para que possamos revisar as mudanças.

## Licença

Este repositório está licenciado sob a **MIT License** - veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

**Contato:**
- Nome: Juliana Geromel
- Email: geromeljuliana@gmail.com
- LinkedIn: (https://www.linkedin.com/in/juliana-geromel/)

