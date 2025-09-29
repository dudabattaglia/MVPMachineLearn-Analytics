 🎧 MVP Machine Learning &amp; Analytics - PUC RIO  -  Maria Eduarda Battaglia  - Setembro 2025


Este projeto foi desenvolvido como entrega do MVP da disciplina **Machine Learning & Analytics**, com o objetivo de prever a popularidade de faixas do Spotify a partir de seus atributos acústicos.

## Estrutura do Projeto
- **MVP_MachineLearning_Spotify.ipynb** — Notebook principal, pronto para execução no Google Colab.
- **dataset.csv** — Dataset com as faixas e atributos (carregado via URL para reprodutibilidade).
- **artifacts/final_model.pkl** — Modelo final treinado (gerado ao executar o notebook).

## Como Executar
1. Abra o [notebook no Google Colab](https://colab.research.google.com/github/dudabattaglia/MVPAnalisedeDados/blob/main/MVP_MachineLearning_Spotify.ipynb).
2. Vá em `Runtime > Run all` para executar todas as células.
3. Verifique no final o RMSE e R² no conjunto de teste.

## Metodologia
- **Problema:** Regressão supervisionada para prever `popularity`.
- **Pré-processamento:** imputação de valores ausentes, padronização, One-Hot Encoding de variáveis categóricas.
- **Modelos Testados:** DummyRegressor (baseline), Linear Regression, Random Forest, XGBoost.
- **Tuning:** RandomizedSearchCV em Random Forest com espaço de busca reduzido para execução rápida.
- **Métricas:** RMSE (principal), R² (complementar).

## Resultados
- Melhor modelo: **Random Forest otimizada**
- RMSE no conjunto de teste: ~0.xx  
- R² no conjunto de teste: ~0.xx  

## Próximos Passos
- Coletar mais dados (ex: engajamento do artista).
- Explorar tuning avançado (n_estimators maiores, max_depth mais profundo).
- Avaliar modelos de boosting mais complexos.

---

📌 **Checklist do MVP:**
- [x] Problema definido e contexto de negócio
- [x] Carga e preparação dos dados
- [x] Divisão treino/validação/teste
- [x] Pipeline de pré-processamento
- [x] Modelagem e baseline
- [x] Otimização de hiperparâmetros
- [x] Avaliação com métricas + análise de erros
- [x] Boas práticas e seed fixa
- [x] Reprodutibilidade
