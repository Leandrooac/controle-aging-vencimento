# Controle de Itens Próximos ao Vencimento — Metodologia de Aging

## Contexto

Como Auxiliar de Controle de Qualidade em uma distribuidora de produtos para saúde, eu precisava acompanhar a proximidade de vencimento de um portfólio de aproximadamente **2.241 SKUs**. As datas de validade existiam no ERP interno da empresa, mas sem classificação de risco e sem um canal estruturado para chegar às áreas que precisavam agir, principalmente vendas e gerência.

O risco de negócio era direto: produtos vencendo sem que a equipe comercial tivesse visibilidade a tempo de agir (promoção, redistribuição ou saída antecipada), gerando perda de estoque.

## Abordagem

1. **Extração**: coleta periódica dos dados de lote e validade direto do ERP interno.
2. **Cálculo de aging**: para cada item, o tempo até o vencimento a partir da data de referência.
3. **Classificação por faixa de risco** (aproximada):

| Faixa (dias) | Classificação |
|---|---|
| -60 a 0 | Vencidos |
| 0 a 30 | Próximo a vencer |
| 30 a 185 | Elegível para valores promocionais de liberação |
| 185 a 365 | Em alerta |
| 365 a 730 | Acompanhar |
| Acima de 730 | Adequado |

> Faixas reconstruídas de memória para documentar a lógica geral. Os parâmetros exatos usados internamente são confidenciais.

4. **Distribuição**: envio quinzenal do controle consolidado para a gerência e as equipes de vendas interna e externa, apoiando decisões de promoção e priorização de saída de estoque.

## Ferramentas

- Microsoft Excel (fórmulas avançadas, formatação condicional)
- Extração de dados de sistema ERP interno

## Resultado

O controle foi adotado pelas áreas comercial e de gerência como parte da rotina de estoque enquanto estive na função. O projeto foi encerrado quando mudei para a área de Comércio Exterior.

A mesma lógica foi reaproveitada depois no [relatório de aging de registros ANVISA](https://github.com/Leandrooac/relatorio-aging-registros-anvisa).

## Sobre os dados neste repositório

Nenhum dado real de produtos, fornecedores ou volumes está incluído. Nome do sistema de origem, valores e identificação de produtos são confidenciais. Este repositório documenta a metodologia, não uma cópia do controle original.
