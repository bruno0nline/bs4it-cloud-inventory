# Arquitetura V1

## Componentes

- AWS Organizations
- Lambda
- S3 Static Website

## Fluxo

Lambda coleta inventário EC2.

Resultado é exportado para:

- inventory.json

Frontend lê inventory.json diretamente do bucket S3.

## Custos previstos

| Serviço | Custo |
|----------|----------|
| S3 | < R$1 |
| Lambda | Free Tier |
| Organizations | Sem custo |

Total estimado: < R$2/mês