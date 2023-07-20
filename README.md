#  Teste para Cientista de Dados
A avaliação consiste em analisar os dados do resultado de uma campanha de marketing de um banco. Para essa avaliação, o candidato deverá utilizar Jupyter Notebook para apresentar seus resultados. [www.kaggle.com/datasets/aaditshukla/bank-marketing-dataset].

# Dados

Os dados são de uma campanha de marketing feita por um banco e estará em csv para o candidato (marketing-banco.csv). A base de dados contém 45211 linhas e 17 atributos. Segue abaixo o metadados de cada atributo:

| Command | Description |
| --- | --- |
| git status | List all new or modified files |
| git diff | Show file differences that haven't been staged |


O primeiro passo é acessar sua conta no Kaggle e obter o arquivo de nome “kaggle.json”. Para isso basta clicar em “My account” no seu avatar no site da plataforma. Click em “Create New API Token” (caso já tenha criado anteriormente, busque o arquivo “kaggle.json”, ou expire-o e gere novas credenciais). Upload o arquivo kaggle.json no Google Colab

```python
! pip install kaggle
! mkdir ~/.kaggle
! cp kaggle.json ~/.kaggle/
! chmod 600 ~/.kaggle/kaggle.json
! kaggle datasets download juniorfazzio/data-of-brazilian-import-and-export-data
```

# Mais informações sobre os dados:

O database apresenta 8 tabelas. Das 8 tabelas, uma tem dados de exportação (exp_completa) e outra de importação (imp_completa). As outras 6 tabelas são tabelas dimensão das tabelas de exportação e importação. (co_ncm, co_pais, cp_unid, cp_urf, _co_via, ncm_unidade).

# Tarefas

Utilizando o Pyspark no Google Colab faça as seguintes tarefas:
- Cria um tabelão com todos os dados relevantes para os dados de exportação e importação;
- Calcule por ano qual o valor FOB de exportação e importação. Após feito isso calcule o a diferença dos dois por ano;
- Identifique qual o país que o Brasil exportar mais e qual o país que o Brasil importar mais de acordo com o valor FOB no ano de 2015.

Esperado que entregue um código no formato .ipynb, estruturado e comentado até 1h antes da entrevista.


