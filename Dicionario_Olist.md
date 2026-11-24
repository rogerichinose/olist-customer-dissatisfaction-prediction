# Dicionário — entradas do modelo e target

Unidade: pedido. Os primeiros 21 atributos são numéricos, os seis seguintes categóricos; a última variável é o target. Ausências são tratadas no pipeline, ajustado no treino.

| Variável | Definição |
|---|---|
| item_count | Quantidade de registros de itens |
| unique_products | Produtos distintos |
| unique_sellers | Vendedores distintos |
| total_price | Soma dos preços em R$ |
| total_freight | Soma do frete em R$ |
| payment_count | Quantidade de registros de pagamento |
| payment_types_count | Tipos distintos de pagamento |
| max_installments | Maior número de parcelas |
| category_count | Categorias distintas de produtos |
| total_weight_g | Soma dos pesos em gramas |
| max_weight_g | Maior peso em gramas |
| total_volume_cm3 | Soma dos volumes em cm³ |
| max_volume_cm3 | Maior volume em cm³ |
| avg_photos_qty | Média da quantidade de fotos |
| avg_description_length | Média do comprimento das descrições |
| same_state_ratio | Proporção de vendedores no mesmo estado do cliente |
| avg_distance_km | Distância média geográfica cliente-vendedor em km |
| approval_delay_hours | Horas entre compra e aprovação |
| estimated_delivery_days | Dias entre compra e entrega estimada |
| freight_ratio | Frete total dividido pelo preço total |
| missing_product_info | Indicador de ausência de fotos ou comprimento da descrição |
| main_payment_type | Tipo do pagamento de maior valor |
| customer_state | UF do cliente |
| main_product_category | Categoria principal do pedido |
| purchase_hour | Hora da compra |
| purchase_dayofweek | Dia da semana da compra (segunda=0) |
| purchase_month | Mês da compra |
| bad_review | 1 para notas 1–2; 0 para notas 3–5 |