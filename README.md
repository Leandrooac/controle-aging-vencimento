# Controle de Itens Próximos ao Vencimento — Metodologia de Aging

## Contexto

Atuando em Assuntos Regulatórios e Qualidade em uma distribuidora de produtos para saúde, era necessário acompanhar a proximidade de vencimento de um portfólio de aproximadamente **2.241 SKUs**. As informações de validade existiam em um sistema ERP interno e caseiro, mas sem classificação de risco nem canal de distribuição estruturado para as áreas que precisavam agir — principalmente vendas e gerência.

O risco de negócio era direto: produtos vencendo sem que a equipe comercial tivesse visibilidade a tempo de agir (promoção, redistribuição ou saída antecipada), gerando perda de estoque.

## Abordagem

1. **Extração**: coleta periódica dos dados de lote e validade diretamente do ERP interno da empresa.
2. **Cálculo de aging**: para cada item, cálculo do tempo até o vencimento a partir da data de referência.
3. **Classificação por faixa de risco**, aproximadamente:

| Faixa (dias) | Classificação |
|---|---|
| -60 a 0 | Vencidos |
| 0 a 30 | Próximo a vencer |
| 30 a 185 | Elegível para criação de valores promocionais de liberação |
| 185 a 365 | Em alerta |
| 365 a 730 | Acompanhar |
| Acima de 730 | Adequado |

> Faixas reconstruídas de memória, para fins de documentação da lógica geral — os parâmetros exatos utilizados internamente pela empresa de origem são confidenciais.

4. **Distribuição**: envio periódico do controle consolidado para gerência e equipes de vendas interna e externa, apoiando decisões de promoção e priorização de saída de estoque.

## Ferramentas

- Microsoft Excel (fórmulas avançadas, formatação condicional)
- Extração de dados de sistema ERP interno

## Resultado

Adoção contínua pelas áreas comercial e de gerência como parte da rotina de controle de estoque. Projeto encerrado com a mudança de função para a área de Comércio Exterior.

## Sobre os dados neste repositório

Nenhum dado real de produtos, fornecedores ou volumes está incluído — nome do sistema de origem, valores e identificação de produtos são informações confidenciais. Este repositório documenta a metodologia do processo, não uma cópia do controle original.
