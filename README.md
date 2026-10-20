# Classificação de Óbitos por COVID-19 com Machine Learning

Atividade em grupo da disciplina de **Inteligência Artificial**: Machine Learning, Parte III.

## Objetivo
Construir e comparar modelos de classificação que preveem se um paciente com COVID-19 evolui para **óbito**, a partir de dados clínicos como idade, sexo, pneumonia, intubação, internação em UTI e comorbidades (diabetes, hipertensão, obesidade, asma, DPOC, insuficiência renal crônica, tabagismo, entre outras).

## Base de dados
**COVID-19 Mexico Patient Health Dataset** (Kaggle, 2020):
https://www.kaggle.com/riteshahlawat/covid19-mexico-patient-health-dataset

## Etapas do projeto
1. **Análise exploratória**: frequência dos atributos, histogramas, resumos estatísticos e mapa de correlação.
2. **Preparação dos dados**: limpeza, tratamento de valores "não se aplica" e "não disponível", e padronização.
3. **Seleção de atributos** com Random Forest (`SelectFromModel`).
4. **Comparação de algoritmos** com validação cruzada estratificada (10 folds):
   - KNN
   - Árvore de Decisão
   - Regressão Logística
   - Naive Bayes
   - SVM
   - Random Forest
   - AdaBoost
5. **Otimização de hiperparâmetros** do melhor modelo (AdaBoost) com `RandomizedSearchCV`.
6. **Avaliação final** com matriz de confusão e relatório de classificação.

## Arquivos
| Arquivo | Descrição |
|---|---|
| `09_IA_EAD_MachineLearning_parteIII_ClassificacaoObitoCOVID_todosAlgoritmos.ipynb` | Notebook principal com todos os algoritmos |
| `IA_EAD_Projeto_COVID19_Classificacao_cv10_atributos.ipynb` | Versão com validação cruzada e seleção de atributos |
| `df_covid.csv` | Base original |
| `df_covid_preparados.csv` | Base após a preparação |
| `dfcovid_atrib_selec.csv` / `dfcovid_atrib_selec_valida.csv` | Bases com os atributos selecionados (treino e validação) |
| `modelo_otimizado_class_obitoCOVID_cv10.sav` | Modelo final treinado e salvo |
| `*.pdf` / `*.docx` | Material de apoio e relatório da atividade |

## Tecnologias
Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn e Jupyter Notebook.

## Como executar
1. Clone o repositório:
   `git clone https://github.com/isah5/Covid.git`
2. Instale as dependências:
   `pip install pandas numpy matplotlib seaborn scikit-learn jupyter`
3. Abra os notebooks com `jupyter notebook`.

## Integrantes
- Isabelle (isah5)
- *(adicione aqui os nomes do grupo)*
