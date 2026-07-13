# Projeto Final - Machine Learning e Visão Computacional

## Predição de Risco de Crédito

### Objetivo

Desenvolver um modelo de Machine Learning capaz de prever a inadimplência de clientes de uma instituição financeira.

---

## Pipeline do Projeto

- Coleta de Dados
- Limpeza Estrutural e Exploração
- Divisão dos Dados
- Pré-processamento
- Treinamento do Modelo
- Avaliação e Validação

---

## Estrutura do Projeto

```text
data/
│
├── raw/
├── processed/

notebooks/

src/

models/

images/

docs/
```

### Tecnologias

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- Git
- GitHub

## Status do Desenvolvimento

### ✔ Etapa 1 - Coleta de Dados

- Importação das bibliotecas
- Carregamento da base
- Verificação inicial
- Inspeção das colunas

## Desenvolvimento

### ✔ Coleta de Dados

- Importação das bibliotecas
- Carregamento da base
- Inspeção inicial
- Auditoria técnica

## Desenvolvimento

### ✔ Coleta de Dados

Concluída

### 🚧 Limpeza Estrutural e Exploração

- Investigação de registros duplicados
- Investigação de valores ausentes

## Status do desenvolvimento

- [x] Estrutura inicial do projeto
- [x] Configuração do ambiente Python
- [x] Coleta e carregamento dos dados
- [x] Auditoria técnica inicial
- [x] Investigação de valores ausentes
- [x] Investigação de registros duplicados
- [x] Análise descritiva e estatística
- [ ] Análise visual das distribuições
- [ ] Análise de outliers
- [ ] Análise da variável alvo
- [ ] Mapa de correlação
- [ ] Tratamento e limpeza
- [ ] Divisão dos dados
- [ ] Pré-processamento
- [ ] Treinamento
- [ ] Avaliação e validação

## Status

✔ Estatística Descritiva

✔ Distribuição da Variável Alvo

🚧 Distribuições Numéricas

## Desenvolvimento

### ✔ Distribuição da Variável Alvo

### ✔ Histogramas das Variáveis Numéricas

Foram analisadas visualmente as distribuições das variáveis contínuas, permitindo identificar possíveis assimetrias e indícios de valores extremos que orientarão as próximas etapas do tratamento dos dados.

- [x] Análise visual das distribuições
- [x] Análise de outliers com boxplots
- [x] Identificação de outliers pelo método IQR
- [ ] Decisão final sobre tratamento dos outliers

## Desenvolvimento

✔ Correlação entre Variáveis

Foi construída uma matriz de correlação de Pearson para investigar relações lineares entre as variáveis numéricas e identificar possíveis atributos com maior influência sobre a variável alvo.

## Status do desenvolvimento

- [x] Coleta de dados
- [x] Análise Exploratória de Dados
- [x] Criação da base de trabalho
- [x] Remoção de registros duplicados
- [x] Reavaliação dos valores ausentes
- [x] Imputação dos valores ausentes
- [x] Tratamento de inconsistências
- [ ] Tratamento de outliers
- [ ] Feature Engineering
- [ ] Divisão dos dados
- [ ] Pré-processamento
- [ ] Treinamento
- [ ] Avaliação e validação

Os valores ausentes de `person_emp_length` e `loan_int_rate` foram imputados com a mediana, pois ambas as variáveis apresentaram assimetria e sensibilidade potencial a valores extremos.

## Status do desenvolvimento

- [x] Coleta de dados
- [x] Análise Exploratória de Dados
- [x] Criação da base de trabalho
- [x] Remoção de registros duplicados
- [x] Reavaliação dos valores ausentes
- [x] Imputação dos valores ausentes
- [x] Tratamento de inconsistências
- [x] Tratamento de outliers
- [ ] Feature Engineering
- [ ] Divisão dos dados
- [ ] Pré-processamento
- [ ] Treinamento
- [ ] Avaliação e validação

Foram removidos registros com idades implausíveis e tempos de emprego incompatíveis com a idade do cliente.

Os outliers financeiros foram mantidos provisoriamente, pois podem representar operações legítimas e relevantes para a predição de inadimplência.


## Status do desenvolvimento

- [x] Coleta de dados
- [x] Análise Exploratória de Dados
- [x] Criação da base de trabalho
- [x] Remoção de registros duplicados
- [x] Reavaliação dos valores ausentes
- [x] Imputação dos valores ausentes
- [x] Tratamento de inconsistências
- [x] Tratamento de outliers
- [ ] Feature Engineering
- [ ] Divisão dos dados
- [ ] Pré-processamento
- [ ] Treinamento
- [ ] Avaliação e validação

Os outliers financeiros foram mantidos por representarem situações plausíveis no contexto de crédito. Apenas inconsistências cadastrais foram removidas, preservando informações relevantes para os modelos de Machine Learning.

## Nova variável criada

Durante a etapa de Feature Engineering, foi criada a variável `comprometimento_renda`, que representa o percentual da renda anual comprometido pelo empréstimo solicitado.

A nova variável será priorizada em relação à coluna original `loan_percent_income` para evitar redundância de informação durante a modelagem.


## Status do desenvolvimento

- [x] Coleta de dados
- [x] Análise Exploratória de Dados
- [x] Criação da base de trabalho
- [x] Remoção de registros duplicados
- [x] Reavaliação dos valores ausentes
- [x] Imputação dos valores ausentes
- [x] Tratamento de inconsistências
- [x] Tratamento de outliers
- [x] Feature Engineering
- [x] Criação da variável `comprometimento_renda`
- [x] Validação de divisão por zero
- [x] Análise de redundância com `loan_percent_income`
- [ ] Definição das variáveis preditoras
- [ ] Divisão dos dados
- [ ] Pré-processamento
- [ ] Treinamento
- [ ] Avaliação e validação
