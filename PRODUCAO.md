# FIORIO BUSINESS INTELLIGENCE — Produção

## Estado consolidado
- 7 abas implementadas: Agendamentos, Entrada de Caixa, Faturamento, TC, Consultas, Marketing e Performance.
- Supabase como banco relacional e autenticação.
- RLS: viewer lê; admin altera. Performance somente admin.
- Relatório Comercial consolidado.
- Exportação de cada aba pelo diálogo nativo de impressão/PDF do navegador.
- Compartilhamento por Web Share API ou cópia de link.

## Variáveis de ambiente
NEXT_PUBLIC_SUPABASE_URL=
NEXT_PUBLIC_SUPABASE_PUBLISHABLE_KEY=

## Publicação recomendada
1. Versionar este diretório em GitHub.
2. Importar o repositório na Vercel como projeto Next.js.
3. Cadastrar as duas variáveis de ambiente acima.
4. Publicar.
5. No Supabase Authentication > URL Configuration, cadastrar a URL publicada e os Redirect URLs.
6. Criar o primeiro usuário no Supabase Auth e promover o perfil para admin.
7. Vincular o domínio `bi.fiorio.com.br` (ou outro desejado) no provedor de hospedagem e apontar o DNS.

## Validação antes da entrada em uso
- Confirmar login/logout.
- Confirmar que viewer não consegue escrever no banco.
- Testar um lançamento em cada módulo e removê-lo em seguida.
- Conferir metas padrão e relatórios.
- Importar dados históricos do Manus somente após a validação funcional.
