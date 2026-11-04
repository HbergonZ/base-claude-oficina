---
name: deploy-vercel
description: Use antes de publicar, quando o deploy na Vercel falhar ou quando for configurar variáveis de ambiente.
---

# Deploy na Vercel

1. Rode `npm run build` e corrija todos os erros de tipo e lint.
2. Confira se cada variável usada no código existe em `.env.example` e na Vercel (Production e Preview).
3. Faça commit com mensagem curta em português e envie para o GitHub.
4. Branch gera link de Preview. Só o que entra na `main` vai para produção, no link público.
5. Se o deploy falhar, leia o log da Vercel, explique a causa em uma frase e corrija.
6. Ao final, informe o link e o que testar nele.
