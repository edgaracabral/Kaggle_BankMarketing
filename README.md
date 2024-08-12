# Kaggle_BankMarketing
## [Kaggle Bank Marketing case](https://www.kaggle.com/datasets/abdelazizsami/bank-marketing/data)

Disponível no Kaggle, esta base de dados é relativa a campanhas de marketing direto de uma instituição financeira Portuguesa, baseadas em chamadas telefônicas. Frequentemente, eram necssários mais de um contato com o mesmo cliente para avaliar se o produto (depósito bancário a prazo) seria ou não subscrito.

Existem três conjuntos de dados:
1) **bank-full.csv** com todos os exemplos (45211) e 17 variáveis de entrada, ordenados por data (de maio de 2008 à novembro de 2010).
2) **bank.csv** com 10% dos exemplos (4521) e 17 variáveis de entrada, selecionados aleatoriamente do conjunto 1.
3) **bank-names.txt** descrição dos dados e citação da referência.

O conjunto de dados menor foi fornecido para testar algoritmos de aprendizado de máquina mais exigentes computacionalmente (por exemplo, SVM).

O objetivo da classificação é prever se o cliente irá subscrever (sim/não) um depósito a prazo (variável y).

Fonte original dos dados:\
[Moro et al., 2011] S. Moro, R. Laureano and P. Cortez. Using Data Mining for Bank Direct Marketing: An Application of the CRISP-DM Methodology. 
  In P. Novais et al. (Eds.), Proceedings of the European Simulation and Modelling Conference - ESM'2011, pp. 117-121, Guimarães, Portugal, October, 2011. EUROSIS.

Available at:
* [pdf] http://hdl.handle.net/1822/14838
* [bib] http://www3.dsi.uminho.pt/pcortez/bib/2011-esm-1.txt

## Estrutura de Pastas no Google Drive
Para se executar estes notebooks, é necessário criar a seguinte estrutura de pastas conforme o caminho indicado:
* `/content/drive/MyDrive/Kaggle/Bank Marketing/00 library`
* `/content/drive/MyDrive/Kaggle/Bank Marketing/01 original data`
* `/content/drive/MyDrive/Kaggle/Bank Marketing/02 data prep`
* `/content/drive/MyDrive/Kaggle/Bank Marketing/03 models`
* `/content/drive/MyDrive/Kaggle/Bank Marketing/12 data prep`
* `/content/drive/MyDrive/Kaggle/Bank Marketing/13 models`

Na pasta '00 library', coloque o arquivo `pod_academy_functions.py`.

Na pasta '01 original data', coloque os arquivos de dados do Kaggle: `bank.csv`, `bank-full.csv` e `bank-names.txt`.

Ao executar-se o notebook '02_Pre_Processamento_de_Dados.ipynb', serão criados os seguintes arquivos na pasta '02 data prep':
* abt_test.csv
* abt_train.csv
* prd_drop_nullvars_hktn.pkl
* prd_fillna_hktn.pkl
* prd_labelenc_hktn.pkl
* prd_list_features_hktn.pkl
* prd_onehotenc_hktn.pkl
* prd_scaler_hktn.pkl

Ao executar-se o notebook '03_Selecao_das_Features.ipynb', serão criados os seguintes arquivos na pasta '02 data prep':
* abt_fs01_train.csv
* abt_fs01_test.csv

Ao executar-se o notebook '04_Construcao_dos_Modelos.ipynb', serão criados os seguintes arquivos na pasta '03 models':
* best_model_dt.pkl
* best_model_rl.pkl
* best_model_rf.pkl
* best_model_lightgbm.pkl

Os notebooks da segunda iteração, '12_Pre_Processamento_de_Dados.ipynb', '13_Selecao_das_Features.ipynb' e '14_Construcao_dos_Modelos.ipynb', criarão os arquivos acima mencionados mas nas pastas '12 data prep' e '13 models'.
