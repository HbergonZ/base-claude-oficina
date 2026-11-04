---
description: Revisa segurança e celular, faz o build, commit e envia para publicar na Vercel.
---

Antes de publicar, revise o diff atual (`git diff`) e corrija o que encontrar:
1. Chaves ou segredos no código ou no commit
2. Tabela nova sem RLS ou sem política
3. Formulário sem validação ou dado do usuário mostrado sem escapar
4. Algo que quebra no celular (largura fixa, texto cortado)
5. Botão "Equipe" faltando em alguma página

Depois siga a skill `deploy-vercel`: build, commit e push. No final, me dê o link para testar.
