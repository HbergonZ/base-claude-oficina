---
name: supabase-seguro
description: Use ao criar ou alterar tabelas, políticas RLS, buckets do Storage ou consultas no Supabase deste projeto.
---

# Supabase com segurança

1. Liste as tabelas que já existem antes de propor mudanças.
2. Escreva o SQL completo (tabela, índices, RLS e políticas) e mostre para a equipe antes de aplicar.
3. Toda tabela: `alter table ... enable row level security;` e uma política para cada operação usada (select, insert, update, delete).
4. Sem login no app? Políticas de leitura pública são ok, mas escrita deve validar o que entra (tamanho de texto, campos obrigatórios).
5. Storage: bucket público só para imagens que todos podem ver. Limite tipo e tamanho do arquivo no upload.
6. No código, use `@supabase/supabase-js` com `NEXT_PUBLIC_SUPABASE_URL` e a chave pública. A service role nunca vai para o navegador.
7. Depois de aplicar, teste com uma consulta simples e conte o resultado para a equipe.
