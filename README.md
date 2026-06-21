# Chems IA — Backend

Servidor que protege a chave do Gemini e comunica com o Supabase em segurança.

## Variáveis de ambiente necessárias

Configura estas variáveis no painel do Render (Settings → Environment):

| Variável | Onde encontrar |
|---|---|
| `GEMINI_API_KEY` | aistudio.google.com/apikey |
| `SUPABASE_URL` | Supabase → Project Settings → API → Project URL |
| `SUPABASE_SERVICE_KEY` | Supabase → Project Settings → API → **Secret key** (nunca a publishable!) |
| `PORT` | Deixa o Render definir automaticamente, ou usa 3000 |

## Rotas disponíveis

- `POST /api/chat` — chat de texto com a IA (sempre grátis, sem limite)
- `POST /api/resolver-foto` — resolução de exercício por foto (10/dia grátis)
- `POST /api/gerar-quiz` — gera 10 perguntas sobre um tema (15 quizzes/dia)
- `POST /api/concluir-quiz` — regista resultado, dá coins e pontos de ranking
- `GET /api/ranking/:tipo` — `geral`, `mensal`, ou `cidades`
- `GET /health` — verifica se o servidor está vivo

Todas as rotas (exceto `/health`) exigem o cabeçalho:
```
Authorization: Bearer <token_de_sessao_do_supabase>
```

## Deploy no Render

1. Sobe este código para um repositório no GitHub
2. No Render: New → Web Service → liga o repositório
3. Build command: `npm install`
4. Start command: `npm start`
5. Adiciona as variáveis de ambiente acima
6. Deploy
