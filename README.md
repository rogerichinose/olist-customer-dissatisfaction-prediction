# Olist — Predição antecipada de insatisfação

Projeto final do MBA TripleTen — Entrega 1.

## Problema
Priorizar pedidos aprovados com risco de avaliação de 1 ou 2 estrelas, para equipes de operações e experiência do cliente. Unidade: pedido. Target binário `bad_review`.

## Dados
[Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce). Baixe os nove CSVs originais e ajuste `data_path` na seção 2.3. Não é necessário publicar os dados brutos no GitHub.

## Execução
Abra `Olist_entrega1_validada.ipynb` no Colab, conecte o Drive e execute todas as células. As dependências estão em `requirements.txt`. O notebook exporta a base elegível e os três conjuntos em `olist_processed/`. Consulte `Dicionario_Olist.md` para as 27 features e o target.

## Indicadores
Average Precision versus prevalência, ROC-AUC, precisão, recall, F1 e lift@K. Impacto monetário e eficácia da intervenção serão avaliados na etapa seguinte; não são resultados comprovados.

## Preparação
Integração por pedido, tratamento de avaliações conflitantes, engenharia de atributos, diagnóstico de ausências e outliers, divisão por aprovação e disponibilidade do target. Treino: 53.699; validação: 17.914; teste: 18.375 pedidos (resultados da execução validada). O EDA complementar inclui correlações e teste Mann–Whitney no treino, executado com 52.088 clientes: p = 1,23022 × 10⁻²⁶, probabilidade de superioridade de 0,5391 e diferença média de 1,20 dia. A associação é fraca e não causal.

## Limitações
Dados históricos, ausência de snapshots de catálogo/pagamento, seleção por disponibilidade de avaliações e exclusividade de clientes. A exploração anterior utilizou a base completa; teste retrospectivo, não independente. Não há demonstração causal de redução de insatisfação.

## Status
Entrega 1: notebook executado sem erros registrados, resultados interpretados e exportações confirmadas. Publicação no GitHub e confirmação formal da aprovação da base externa com tutor pendentes. Modelagem e otimização serão entregues posteriormente.
