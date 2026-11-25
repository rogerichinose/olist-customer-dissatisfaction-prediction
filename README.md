# Olist — Predição antecipada de insatisfação

Entrega 2 — Etapas 1, 2 e 3 do MBA TripleTen.

## Execução
Baixe os nove CSVs do [dataset Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce), abra `Olist_entrega2_revisada.ipynb` no Colab, ajuste `data_path` e execute todas as células. A limpeza estadual consulta a API de malhas do IBGE.

## Revisão solicitada
Diagnóstico de faltantes corrigido e recalculado; gráficos de status, sazonalidade, distribuições e extremos; validação geográfica por UF e CEP; exportação dos quatro CSVs com tamanho informado. Copie `olist_processed/` após execução, observando o limite de arquivos e a licença dos dados.

## Modelagem
Baseline, regressão logística, Random Forest e LightGBM; avaliação temporal retrospectiva, AP, ROC-AUC, F1 e lift; simulação econômica, planejamento A/B, Optuna, SHAP e análise de disparidades. Os resultados atualizados estão na seção 12 após execução. Não há validação prospectiva nem impacto causal comprovado.

## Status
Código revisado, ainda não executado com os CSVs originais. Antes de enviar, execute tudo, revise as conclusões históricas sinalizadas e confirme os resultados. A etapa opcional de deploy não integra esta entrega.
