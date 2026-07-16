# Projeto Final — Machine Learning e Visão Computacional

Pipeline completo para previsão de risco de crédito utilizando técnicas de Ciência de Dados, Engenharia de Atributos e algoritmos clássicos de Machine Learning.

## Objetivo

Desenvolver um pipeline completo de Machine Learning capaz de prever a inadimplência de clientes em solicitações de crédito, aplicando boas práticas de preparação de dados, engenharia de atributos, modelagem, otimização de hiperparâmetros e avaliação estatística.

O projeto foi desenvolvido como parte da Situação de Aprendizagem do módulo de Machine Learning e Visão Computacional.

## Problema de Negócio

Instituições financeiras precisam reduzir perdas provocadas pela concessão de crédito para clientes inadimplentes.

O objetivo deste projeto é desenvolver um modelo preditivo capaz de classificar clientes como:

- Adimplentes (loan_status = 0)
- Inadimplentes (loan_status = 1)

A solução proposta auxilia o banco na tomada de decisão durante a análise de crédito, reduzindo riscos financeiros e aumentando a eficiência do processo.

## Dataset

Base utilizada:

**Loan Risk Dataset**

Principais informações:

- Dados financeiros dos clientes
- Informações pessoais
- Histórico de crédito
- Características do empréstimo
- Status final do pagamento

## Estrutura do Projeto

carreira-tec-machine-learning-projeto-final/

│

├── data/

├── docs/

├── images/

├── models/

├── notebooks/

│   └── projeto_final.ipynb

├── src/

├── README.md

├── requirements.txt

└── LICENSE

## Tecnologias Utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- Imbalanced-Learn
- Jupyter Notebook
- VS Code
- Git
- GitHub

## Pipeline de Machine Learning

O desenvolvimento seguiu o fluxo:

1. Coleta dos Dados

2. Limpeza Estrutural e Exploração

3. Tratamento e Limpeza dos Dados

4. Feature Engineering

5. Divisão dos Dados
 
6. Pré-processamento

7. Modelagem

8. Avaliação Final

9. Veredito Final

## Dicionário de Dados

| Coluna | Descrição |
|---------|-----------|
| person_age | Idade do cliente |
| person_income | Renda anual |
| person_home_ownership | Situação do imóvel |
| person_emp_length | Tempo de emprego |
| loan_amnt | Valor do empréstimo |
| loan_int_rate | Taxa de juros |
| loan_intent | Finalidade do empréstimo |
| loan_grade | Classificação do empréstimo |
| cb_person_cred_hist_length | Tempo de histórico de crédito |
| loan_status | Variável alvo |
| comprometimento_renda | Percentual da renda comprometido pelo empréstimo (variável criada) |

## Metodologia

Durante o desenvolvimento foram executadas as seguintes etapas:

- Análise Exploratória de Dados (EDA)
- Tratamento de valores ausentes
- Remoção de registros duplicados
- Investigação de outliers
- Feature Engineering
- One-Hot Encoding
- Divisão estratificada em treino e teste
- Balanceamento com SMOTE
- Escalonamento com StandardScaler para o KNN
- Treinamento dos modelos
- Otimização de hiperparâmetros
- Avaliação com Classification Report
- Matrizes de Confusão
- Análise de impacto de negócio

## Resultados Obtidos

### Melhor KNN

- Parâmetro: K = 9
- Accuracy: 88,32%

### Melhor Árvore

- Profundidade: 7
- Accuracy: 92,59%

## Modelo Selecionado

Após a comparação entre os algoritmos avaliados, a Árvore de Decisão com profundidade máxima igual a 7 foi selecionada como modelo final.

Principais motivos:

- maior acurácia no conjunto de teste;
- excelente capacidade de generalização;
- menor diferença entre treino e teste;
- menor número de falsos positivos;
- menor número de falsos negativos.

Sob a ótica do negócio, apresentou menor risco financeiro para a instituição bancária.

## Como executar

Clone o repositório:

git clone <https://github.com/MayconValer/carreira-tec-machine-learning-projeto-final.git>

Intale as dependencias:

pip install -r requirements.txt

Abra:

notebooks/projeto_final.ipynb

Execute todas as células na ordem apresentada.


---

# 13. Histórico do Projeto

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
- [x]  Definição das variáveis preditoras
- [x] Divisão estratificada dos dados
- [x] Identificação das variáveis categóricas e numéricas
- [x] One-Hot Encoding ajustado somente no treino
- [x] Transformação segura do conjunto de teste
- [x] One-Hot Encoding
- [x] Balanceamento com SMOTE apenas no treino
- [x] Preservação da distribuição original do teste
- [x] Escalonamento seguro para KNN
- [x] Base preparada para Árvore de Decisão
- [x] Pré-processamento
- [x] Início da Modelagem
- [x] Primeiro treinamento do KNN
- [x] Otimização do KNN
- [x] Comparação entre diferentes valores de K
- [x] Diagnóstico inicial de Overfitting
- [x] Otimização do KNN
- [x] Otimização da Árvore
- [x] Diagnóstico de Overfitting
- [x] Comparação entre modelos
- [x] Seleção automática das melhores configurações
- [x] Classification Report
- [x] Matrizes de Confusão
- [x] Interpretação dos erros
- [x] Avaliação
- [x] Veredito Executivo


## Versionamento

O desenvolvimento foi realizado utilizando Git Flow simplificado.

Branches utilizadas:

- main
- fase/coleta-dados
- fase/eda
- fase/data-prep
- fase/feature-engineering
- fase/divisao-dados
- fase/pre-processamento
- fase/modelagem
- fase/documentacao-final

## Autor

Maycon Diego Valer

Projeto desenvolvido para a disciplina:

Machine Learning e Visão Computacional

Carreira Tech


## 🎥 Apresentação do Projeto

A apresentação completa do desenvolvimento do projeto pode ser assistida no YouTube:

Projeto Final — Machine Learning para Risco de Crédito | Maycon Valer

https://youtu.be/UHqmH5g7rv8?si=Eroo0naWW7nn-GFW
