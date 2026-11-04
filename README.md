# Base da oficina: do prompt ao deploy

Modelo de repositório para os projetos da oficina Conexão Tech.RO.

## O que tem aqui
| Arquivo | Para quê |
|---|---|
| `CLAUDE.md` | Regras do projeto que o Claude lê em toda sessão |
| `AGENTS.md` | Aponta o Codex para as mesmas regras |
| `.claude/skills/` | `supabase-seguro` e `deploy-vercel`, usadas quando o assunto aparece |
| `.claude/commands/` | `/proximo-passo` e `/publicar` |
| `.claude/settings.json` | Libera build e lint e bloqueia a leitura do `.env` |
| `.mcp.json` | Supabase e Vercel para quem usa o Claude Code no terminal |

## Como usar
Este é um repositório modelo. Ele começa sem app: na primeira sessão o Claude cria o Next.js na raiz, mantendo estes arquivos.

1. Clique em **Use this template → Create a new repository** e crie o repositório da equipe.
2. Abra **claude.ai/code**, escolha o repositório e ligue os conectores do Supabase e da Vercel. No Codex, conecte o mesmo repositório.
3. Cole o prompt inicial da ideia escolhida, com a linha Equipe preenchida.
4. Siga com `/proximo-passo` e, para publicar, `/publicar`.
