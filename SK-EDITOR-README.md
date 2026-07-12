# SK Code Editor — Source Code

Editor de código mobile-first criado pelo Saulo Kenji.
PWA instalável (Android/iOS), funciona offline, com IA Jasmim integrada.

## ESTRUTURA

artifacts/code-editor/  → PWA Frontend (React + Vite + Monaco Editor)
artifacts/api-server/   → Backend (Express + TypeScript) — Jasmim usa
lib/                    → Bibliotecas compartilhadas (api-client, db)
package.json            → raiz do monorepo pnpm
pnpm-workspace.yaml     → config workspace
replit.md               → documentação do projeto

## RODAR LOCALMENTE

# 1. Instalar pnpm
npm install -g pnpm

# 2. Instalar dependências
pnpm install

# 3. Rodar tudo
pnpm --filter @workspace/code-editor run dev   # PWA em http://localhost:5173
pnpm --filter @workspace/api-server run dev    # API em http://localhost:8080

## VARIÁVEIS DE AMBIENTE PRA JASMIM (IA)

AI_INTEGRATIONS_OPENAI_BASE_URL — URL do provedor OpenAI-compatível
AI_INTEGRATIONS_OPENAI_API_KEY  — chave de API

## TECNOLOGIAS

- React 18 + Vite 7 + TypeScript
- Monaco Editor (mesmo do VSCode)
- Tailwind CSS
- Express 4
- Service Worker (PWA + COOP/COEP pra WebContainer)
- Modelos GPT-5.4 via integração OpenAI

## FUNCIONALIDADES PRINCIPAIS

- Editor Monaco com syntax highlighting
- Terminal triplo: Online (servidor) / Real (WebContainer Node-no-navegador) / Offline (simulado)
- Jasmim (IA) com acesso ao terminal, arquivos, web search
- Comandos de voz (entrada e saída)
- PWA instalável com auto-atualização (sem ficar preso em versão antiga)
- Integração GitHub
- Banco de dados PostgreSQL

## NOTAS

- O Service Worker (artifacts/code-editor/public/sw.js) usa estratégia
  network-first pra HTML e cache-first pra assets com hash, garantindo
  updates automáticos após cada deploy.
- Mobile-first: feito pra usar com voz no celular.
