# FIORIO BUSINESS INTELLIGENCE — Sprint 1

Primeira versão web própria do painel Fiorio.

## Entregue nesta sprint
- Next.js 16.3 + Supabase SSR
- Login por e-mail/senha
- Papéis `admin` e `viewer` respeitando RLS no PostgreSQL
- Identidade visual Fiorio (dark + azul/ciano)
- Navegação com as 7 áreas do BI; Performance fica oculta para viewer
- Aba Agendamentos conectada ao banco
- KPIs do mês: Agendados, Realizados, Vagas, Prioritários e Ocupação
- CRUD de agendamentos somente para admin
- Status interno `confirmado` exibido como `Realizado`
- Seletor independente de mês/ano
- Alertas de vagas prioritárias
- Banco completo da fundação incluído em `supabase/schema.sql`

## Como ligar o projeto
1. Crie um projeto Supabase.
2. No SQL Editor, rode `supabase/schema.sql` e depois `supabase/bootstrap.sql`.
3. Em Authentication > Users, crie seu usuário.
4. Copie o UUID do usuário e execute: `update public.profiles set role='admin' where id='SEU_UUID';`
5. Copie `.env.example` para `.env.local` e preencha URL e Publishable Key.
6. Rode `npm install` e `npm run dev`.

## Próxima sprint
Conectar Entrada de Caixa e Faturamento, incluindo metas editáveis, regra da última semana positiva, semáforos de risco, histórico anual e PDF.


## Sprint 2
Entrada de Caixa e Faturamento agora estão funcionais e persistentes. Consulte `SPRINT2.md`.


## Sprint 3
Módulo TC Realizados × Agendados implementado com metas independentes, ticket médio, conversão complementar e IP de 60 dias / 26.

## Versão consolidada de produção
A versão atual reúne Sprints 1–6. Consulte `PRODUCAO.md` para publicação e checklist de entrada em uso.
