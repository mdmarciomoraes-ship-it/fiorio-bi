# Sprint 1 — decisão arquitetural

O objetivo desta etapa é tirar o núcleo operacional do Manus e colocá-lo em uma aplicação própria, com autenticação e persistência reais.

## Regra preservada
- `confirmado` permanece como valor interno para compatibilidade, mas a interface mostra `Realizado`.
- `admin` pode criar/editar/excluir; `viewer` somente lê.
- Performance é invisível a `viewer`.
- A meta de ocupação mensal padrão é 13, podendo vir de `monthly_goals`.
- Todas as alterações de dados dependem de RLS do banco, não apenas de botões escondidos.

## Próxima implementação
1. Caixa
2. Faturamento
3. TC Realizados × Agendados
4. Consultas
5. Marketing
6. Performance
7. PDFs e Relatório Comercial
