# FIORIO BI · Sprint 2

## Entregue
- Módulo Entrada de Caixa conectado ao Supabase.
- Módulo Faturamento conectado ao Supabase.
- Seletor de mês/ano independente em cada módulo.
- Lançamentos semanais com semanas dinâmicas.
- Edição e exclusão restritas ao admin; viewer somente leitura.
- Metas mensais configuráveis por período.
- Caixa: R$ 75 mil/semana, R$ 300 mil/mês, metas R$ 350/400/450 mil.
- Faturamento: R$ 87,5 mil/semana, R$ 350 mil/mês, metas R$ 400/500/600 mil.
- Indicadores de meta semanal, desvio de ritmo e risco mensal.
- Regra de diagnóstico baseada na última semana com lançamento positivo.
- Gráfico visual semanal com linha de meta.
- Histórico anual dos acumulados mensais.
- KPIs de acumulado, falta para meta, percentual e próxima meta.

## Regra crítica preservada
Quando a última semana positiva fica abaixo da meta semanal, o painel mostra:
- Meta semanal mínima atingida? NÃO.
- Desvio de ritmo identificado? SIM (vermelho).
- Risco de não bater a meta mensal? SIM (vermelho).
