# PLANO DO PROJETO: sk-editor-source

> Gerado automaticamente pelo SK Code Editor em 12/07/2026, 13:30:44
> **149 arquivo(s)** | **~35.063 linhas de codigo**

---

## RESUMO EXECUTIVO

- **Tipo de aplicacao:** Aplicacao Web Frontend (React)
- **Frontend / Stack principal:** React, TypeScript
- **Versao:** 0.0.0

**Para rodar o projeto:**
```bash
# Abra index.html no Preview (botao Play)
```

---

## ESTRUTURA DE ARQUIVOS

```
sk-editor-source/
├── artifacts/
│   ├── api-server/
│   │   ├── .replit-artifact/
│   │   │   └── artifact.toml
│   │   ├── src/
│   │   │   ├── lib/
│   │   │   │   └── logger.ts
│   │   │   ├── routes/
│   │   │   │   ├── ai-chat.ts
│   │   │   │   ├── ai-forward.ts
│   │   │   │   ├── config.ts
│   │   │   │   ├── db.ts
│   │   │   │   ├── drive.ts
│   │   │   │   ├── exec.ts
│   │   │   │   ├── github.ts
│   │   │   │   ├── health.ts
│   │   │   │   ├── index.ts
│   │   │   │   ├── legal-ai.ts
│   │   │   │   ├── proxy.ts
│   │   │   │   ├── search.ts
│   │   │   │   ├── twa.ts
│   │   │   │   ├── upload.ts
│   │   │   │   ├── voice.ts
│   │   │   │   └── workspace.ts
│   │   │   ├── app.ts
│   │   │   └── index.ts
│   │   ├── build.mjs
│   │   ├── package.json
│   │   ├── pty_helper.c
│   │   └── tsconfig.json
│   └── code-editor/
│       ├── .replit-artifact/
│       │   └── artifact.toml
│       ├── public/
│       │   ├── favicon.svg
│       │   ├── guia-completo-apk.md
│       │   ├── manifest.json
│       │   └── sw.js
│       ├── src/
│       │   ├── components/
│       │   │   ├── ui/
│       │   │   │   ├── accordion.tsx
│       │   │   │   ├── alert-dialog.tsx
│       │   │   │   ├── alert.tsx
│       │   │   │   ├── aspect-ratio.tsx
│       │   │   │   ├── avatar.tsx
│       │   │   │   ├── badge.tsx
│       │   │   │   ├── breadcrumb.tsx
│       │   │   │   ├── button-group.tsx
│       │   │   │   ├── button.tsx
│       │   │   │   ├── calendar.tsx
│       │   │   │   ├── card.tsx
│       │   │   │   ├── carousel.tsx
│       │   │   │   ├── chart.tsx
│       │   │   │   ├── checkbox.tsx
│       │   │   │   ├── collapsible.tsx
│       │   │   │   ├── command.tsx
│       │   │   │   ├── context-menu.tsx
│       │   │   │   ├── dialog.tsx
│       │   │   │   ├── drawer.tsx
│       │   │   │   ├── dropdown-menu.tsx
│       │   │   │   ├── empty.tsx
│       │   │   │   ├── field.tsx
│       │   │   │   ├── form.tsx
│       │   │   │   ├── hover-card.tsx
│       │   │   │   ├── input-group.tsx
│       │   │   │   ├── input-otp.tsx
│       │   │   │   ├── input.tsx
│       │   │   │   ├── item.tsx
│       │   │   │   ├── kbd.tsx
│       │   │   │   ├── label.tsx
│       │   │   │   ├── menubar.tsx
│       │   │   │   ├── navigation-menu.tsx
│       │   │   │   ├── pagination.tsx
│       │   │   │   ├── popover.tsx
│       │   │   │   ├── progress.tsx
│       │   │   │   ├── radio-group.tsx
│       │   │   │   ├── resizable.tsx
│       │   │   │   ├── scroll-area.tsx
│       │   │   │   ├── select.tsx
│       │   │   │   ├── separator.tsx
│       │   │   │   ├── sheet.tsx
│       │   │   │   ├── sidebar.tsx
│       │   │   │   ├── skeleton.tsx
│       │   │   │   ├── slider.tsx
│       │   │   │   ├── sonner.tsx
│       │   │   │   ├── spinner.tsx
│       │   │   │   ├── switch.tsx
│       │   │   │   ├── table.tsx
│       │   │   │   ├── tabs.tsx
│       │   │   │   ├── textarea.tsx
│       │   │   │   ├── toast.tsx
│       │   │   │   ├── toaster.tsx
│       │   │   │   ├── toggle-group.tsx
│       │   │   │   ├── toggle.tsx
│       │   │   │   └── tooltip.tsx
│       │   │   ├── AIChat.tsx
│       │   │   ├── AssistenteJuridico.tsx
│       │   │   ├── CampoLivre.tsx
│       │   │   ├── CodeEditor.tsx
│       │   │   ├── CombinarApps.tsx
│       │   │   ├── DriveBackupPanel.tsx
│       │   │   ├── EditorLayout.tsx
│       │   │   ├── FileTree.tsx
│       │   │   ├── GitHubPanel.tsx
│       │   │   ├── Manual.tsx
│       │   │   ├── PackageSearch.tsx
│       │   │   ├── Preview.tsx
│       │   │   ├── QuickPrompt.tsx
│       │   │   ├── RealTerminal.tsx
│       │   │   ├── StreamTerminal.tsx
│       │   │   ├── SystemStatusPanel.tsx
│       │   │   ├── TemplateSelector.tsx
│       │   │   ├── Terminal.tsx
│       │   │   ├── VoiceCard.tsx
│       │   │   ├── VoiceMode.tsx
│       │   │   └── WebContainerTerminal.tsx
│       │   ├── hooks/
│       │   │   ├── use-mobile.tsx
│       │   │   └── use-toast.ts
│       │   ├── lib/
│       │   │   ├── ai-service.ts
│       │   │   ├── github-service.ts
│       │   │   ├── projects.ts
│       │   │   ├── store.ts
│       │   │   ├── templates.ts
│       │   │   ├── tts-service.ts
│       │   │   ├── utils.ts
│       │   │   ├── virtual-fs.ts
│       │   │   └── zip-service.ts
│       │   ├── App.tsx
│       │   ├── index.css
│       │   └── main.tsx
│       ├── components.json
│       ├── index.html
│       ├── package.json
│       ├── SYSTEM_DOCS.md
│       ├── tsconfig.json
│       └── vite.config.ts
├── lib/
│   ├── api-client-react/
│   │   ├── src/
│   │   │   ├── generated/
│   │   │   │   ├── api.schemas.ts
│   │   │   │   └── api.ts
│   │   │   ├── custom-fetch.ts
│   │   │   └── index.ts
│   │   ├── package.json
│   │   └── tsconfig.json
│   ├── api-spec/
│   │   ├── openapi.yaml
│   │   ├── orval.config.ts
│   │   └── package.json
│   ├── api-zod/
│   │   ├── src/
│   │   │   ├── generated/
│   │   │   │   ├── types/
│   │   │   │   │   ├── healthStatus.ts
│   │   │   │   │   └── index.ts
│   │   │   │   └── api.ts
│   │   │   └── index.ts
│   │   ├── package.json
│   │   └── tsconfig.json
│   └── db/
│       ├── src/
│       │   ├── schema/
│       │   │   └── index.ts
│       │   └── index.ts
│       ├── drizzle.config.ts
│       ├── package.json
│       └── tsconfig.json
├── package.json
├── pnpm-workspace.yaml
├── replit.md
└── SK-EDITOR-README.md
```

---

## STACK TECNOLOGICO DETECTADO

- **Frontend:** React, TypeScript
- **Todos os pacotes (2):** typescript, prettier

---

## ROTAS DA API (endpoints detectados automaticamente)

```
USE    /api  (em artifacts/api-server/src/app.ts)
GET    /ai/chat  (em artifacts/api-server/src/routes/ai-chat.ts)
POST   /ai/chat  (em artifacts/api-server/src/routes/ai-chat.ts)
POST   /ai/forward  (em artifacts/api-server/src/routes/ai-forward.ts)
GET    /config  (em artifacts/api-server/src/routes/config.ts)
POST   /db/neon/create  (em artifacts/api-server/src/routes/db.ts)
GET    /db/neon/projects  (em artifacts/api-server/src/routes/db.ts)
POST   /db/neon/credentials  (em artifacts/api-server/src/routes/db.ts)
POST   /db/execute  (em artifacts/api-server/src/routes/db.ts)
POST   /db/test-connection  (em artifacts/api-server/src/routes/db.ts)
GET    /drive/list  (em artifacts/api-server/src/routes/drive.ts)
POST   /drive/upload  (em artifacts/api-server/src/routes/drive.ts)
DELETE /drive/delete/:fileId  (em artifacts/api-server/src/routes/drive.ts)
POST   /exec/npm-install  (em artifacts/api-server/src/routes/exec.ts)
POST   /exec/run-node  (em artifacts/api-server/src/routes/exec.ts)
POST   /exec/run-node-vfs  (em artifacts/api-server/src/routes/exec.ts)
POST   /db/query  (em artifacts/api-server/src/routes/exec.ts)
POST   /projects/:projectId/exec-stream  (em artifacts/api-server/src/routes/exec.ts)
GET    /github/user  (em artifacts/api-server/src/routes/github.ts)
GET    /github/repos  (em artifacts/api-server/src/routes/github.ts)
POST   /github/repos  (em artifacts/api-server/src/routes/github.ts)
POST   /github/push  (em artifacts/api-server/src/routes/github.ts)
DELETE /github/repos/:owner/:repo  (em artifacts/api-server/src/routes/github.ts)
GET    /healthz  (em artifacts/api-server/src/routes/health.ts)
USE    /voice  (em artifacts/api-server/src/routes/index.ts)
POST   /legal/process  (em artifacts/api-server/src/routes/legal-ai.ts)
POST   /legal/refine  (em artifacts/api-server/src/routes/legal-ai.ts)
GET    /search  (em artifacts/api-server/src/routes/search.ts)
GET    /npm-search  (em artifacts/api-server/src/routes/search.ts)
GET    /pwa-check  (em artifacts/api-server/src/routes/twa.ts)
GET    /twa-files  (em artifacts/api-server/src/routes/twa.ts)
POST   /upload/extract-text  (em artifacts/api-server/src/routes/upload.ts)
POST   /transcribe  (em artifacts/api-server/src/routes/voice.ts)
POST   /speak  (em artifacts/api-server/src/routes/voice.ts)
GET    /workspace/info  (em artifacts/api-server/src/routes/workspace.ts)
POST   /workspace/write  (em artifacts/api-server/src/routes/workspace.ts)
GET    /workspace/read  (em artifacts/api-server/src/routes/workspace.ts)
GET    /workspace/list  (em artifacts/api-server/src/routes/workspace.ts)
POST   /workspace/delete  (em artifacts/api-server/src/routes/workspace.ts)
POST   /workspace/install  (em artifacts/api-server/src/routes/workspace.ts)
POST   /workspace/run  (em artifacts/api-server/src/routes/workspace.ts)
POST   /workspace/sync  (em artifacts/api-server/src/routes/workspace.ts)
GET    /api/items  (em artifacts/code-editor/src/lib/templates.ts)
GET    /api/items/:id  (em artifacts/code-editor/src/lib/templates.ts)
POST   /api/items  (em artifacts/code-editor/src/lib/templates.ts)
GET    /api/health  (em artifacts/code-editor/src/lib/templates.ts)
USE    /api/auth  (em artifacts/code-editor/src/lib/templates.ts)
USE    /api/usuarios  (em artifacts/code-editor/src/lib/templates.ts)
POST   /register  (em artifacts/code-editor/src/lib/templates.ts)
POST   /login  (em artifacts/code-editor/src/lib/templates.ts)
GET    /perfil  (em artifacts/code-editor/src/lib/templates.ts)
GET    /api/provedores  (em artifacts/code-editor/src/lib/templates.ts)
POST   /api/chat  (em artifacts/code-editor/src/lib/templates.ts)
GET    /health  (em artifacts/code-editor/src/lib/templates.ts)
POST   /auth/login  (em artifacts/code-editor/src/lib/templates.ts)
POST   /auth/registro  (em artifacts/code-editor/src/lib/templates.ts)
GET    /clientes  (em artifacts/code-editor/src/lib/templates.ts)
GET    /clientes/:id  (em artifacts/code-editor/src/lib/templates.ts)
POST   /clientes  (em artifacts/code-editor/src/lib/templates.ts)
PUT    /clientes/:id  (em artifacts/code-editor/src/lib/templates.ts)
GET    /processos  (em artifacts/code-editor/src/lib/templates.ts)
GET    /processos/:id  (em artifacts/code-editor/src/lib/templates.ts)
POST   /processos  (em artifacts/code-editor/src/lib/templates.ts)
GET    /audiencias  (em artifacts/code-editor/src/lib/templates.ts)
POST   /audiencias  (em artifacts/code-editor/src/lib/templates.ts)
GET    /prazos/proximos  (em artifacts/code-editor/src/lib/templates.ts)
GET    /dashboard  (em artifacts/code-editor/src/lib/templates.ts)
GET    /api/registros  (em artifacts/code-editor/src/lib/templates.ts)
GET    /api/registros/:id  (em artifacts/code-editor/src/lib/templates.ts)
POST   /api/registros  (em artifacts/code-editor/src/lib/templates.ts)
PUT    /api/registros/:id  (em artifacts/code-editor/src/lib/templates.ts)
DELETE /api/registros/:id  (em artifacts/code-editor/src/lib/templates.ts)
```

---

## SCRIPTS DISPONIVEIS (package.json)

```bash
npm run preinstall    # sh -c 'rm -f package-lock.json yarn.lock; case "$npm_config_user_agent" in pnpm/*) ;; *) echo "Use pnpm instead" >&2; exit 1 ;; esac'
npm run build         # pnpm run typecheck && pnpm -r --if-present run build
npm run typecheck:libs  # tsc --build
npm run typecheck     # pnpm run typecheck:libs && pnpm -r --filter "./artifacts/**" --filter "./scripts" --if-present run typecheck
```

---

## VARIAVEIS DE AMBIENTE NECESSARIAS

Crie um arquivo `.env` na raiz com estas variaveis:

```env
LOG_LEVEL=seu_valor_aqui
DATABASE_URL=seu_valor_aqui
AI_INTEGRATIONS_OPENAI_BASE_URL=seu_valor_aqui
AI_INTEGRATIONS_OPENAI_API_KEY=seu_valor_aqui
PORT=seu_valor_aqui
ALLOWED_ORIGINS=seu_valor_aqui
JWT_SECRET=seu_valor_aqui
JWT_EXPIRES_IN=seu_valor_aqui
GROQ_API_KEY=seu_valor_aqui
OPENAI_API_KEY=seu_valor_aqui
GEMINI_API_KEY=seu_valor_aqui
ANTHROPIC_API_KEY=seu_valor_aqui
XAI_API_KEY=seu_valor_aqui
OPENROUTER_API_KEY=seu_valor_aqui
PERPLEXITY_API_KEY=seu_valor_aqui
TELEGRAM_TOKEN=seu_valor_aqui
BASE_PATH=seu_valor_aqui
REPL_ID=seu_valor_aqui
```

---

## ARQUIVOS PRINCIPAIS

- `artifacts/api-server/src/app.ts` — Ponto de entrada do backend
- `artifacts/api-server/src/index.ts` — Ponto de entrada do backend
- `artifacts/api-server/src/routes/index.ts` — Ponto de entrada do backend
- `artifacts/code-editor/index.html` — Arquivo principal
- `artifacts/code-editor/src/App.tsx` — Componente raiz do frontend
- `artifacts/code-editor/src/main.tsx` — Arquivo principal
- `lib/api-client-react/src/index.ts` — Arquivo principal
- `lib/api-zod/src/generated/types/index.ts` — Arquivo principal
- `lib/api-zod/src/index.ts` — Arquivo principal
- `lib/db/src/index.ts` — Arquivo principal

---

## GUIA COMPLETO — O QUE CADA PARTE DO PROJETO FAZ

> Esta secao explica, em linguagem simples, o que e para que serve cada pasta e cada arquivo.

### 📁 Raiz do Projeto (pasta principal)
> Arquivos de configuracao e pontos de entrada ficam aqui.

**`SK-EDITOR-README.md`** _(57 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`package.json`** _(33 linhas)_
Registro de dependencias e scripts do projeto. Aqui ficam os comandos (npm run dev, npm start) e os pacotes instalados.

**`pnpm-workspace.yaml`** _(160 linhas)_
Arquivo YAML — parte do projeto.

**`replit.md`** _(65 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `artifacts/api-server/`
> Pasta 'api-server' — agrupamento de arquivos relacionados.

**`build.mjs`** _(159 linhas)_
Arquivo MJS — parte do projeto.

**`package.json`** _(46 linhas)_
Registro de dependencias e scripts do projeto. Aqui ficam os comandos (npm run dev, npm start) e os pacotes instalados.

**`pty_helper.c`** _(138 linhas)_
Arquivo C — parte do projeto.

**`tsconfig.json`** _(18 linhas)_
Configuracao do TypeScript. Diz para o computador como interpretar o codigo .ts e .tsx.

---

### 📁 `artifacts/code-editor/`
> Pasta 'code-editor' — agrupamento de arquivos relacionados.

**`SYSTEM_DOCS.md`** _(292 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`components.json`** _(20 linhas)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

**`index.html`** _(98 linhas)_
Pagina HTML raiz do projeto. E o ponto de entrada que o browser carrega primeiro.

**`package.json`** _(93 linhas)_
Registro de dependencias e scripts do projeto. Aqui ficam os comandos (npm run dev, npm start) e os pacotes instalados.

**`tsconfig.json`** _(23 linhas)_
Configuracao do TypeScript. Diz para o computador como interpretar o codigo .ts e .tsx.

**`vite.config.ts`** _(69 linhas)_
Configuracao do Vite (servidor de desenvolvimento). Define a porta, alias de caminhos e plugins usados.

---

### 📁 `lib/api-client-react/`
> Pasta 'api-client-react' — agrupamento de arquivos relacionados.

**`package.json`** _(16 linhas)_
Registro de dependencias e scripts do projeto. Aqui ficam os comandos (npm run dev, npm start) e os pacotes instalados.

**`tsconfig.json`** _(13 linhas)_
Configuracao do TypeScript. Diz para o computador como interpretar o codigo .ts e .tsx.

---

### 📁 `lib/api-spec/`
> Pasta 'api-spec' — agrupamento de arquivos relacionados.

**`openapi.yaml`** _(37 linhas)_
Arquivo YAML — parte do projeto.

**`orval.config.ts`** _(73 linhas)_
Arquivo de CONSTANTES/CONFIGURACAO — valores fixos usados em varios lugares do projeto.

**`package.json`** _(12 linhas)_
Registro de dependencias e scripts do projeto. Aqui ficam os comandos (npm run dev, npm start) e os pacotes instalados.

---

### 📁 `lib/api-zod/`
> Pasta 'api-zod' — agrupamento de arquivos relacionados.

**`package.json`** _(13 linhas)_
Registro de dependencias e scripts do projeto. Aqui ficam os comandos (npm run dev, npm start) e os pacotes instalados.

**`tsconfig.json`** _(12 linhas)_
Configuracao do TypeScript. Diz para o computador como interpretar o codigo .ts e .tsx.

---

### 📁 `lib/db/`
> Pasta 'db' — agrupamento de arquivos relacionados.

**`drizzle.config.ts`** _(15 linhas)_
Configuracao do Drizzle ORM — gerencia a conexao e migracao do banco de dados.

**`package.json`** _(26 linhas)_
Registro de dependencias e scripts do projeto. Aqui ficam os comandos (npm run dev, npm start) e os pacotes instalados.

**`tsconfig.json`** _(13 linhas)_
Configuracao do TypeScript. Diz para o computador como interpretar o codigo .ts e .tsx.

---

### 📁 `artifacts/api-server/.replit-artifact/`
> Pasta '.replit-artifact' — agrupamento de arquivos relacionados.

**`artifact.toml`** _(33 linhas)_
Arquivo TOML — parte do projeto.

---

### 📁 `artifacts/api-server/src/`
> Codigo-fonte principal do projeto. Nao apague esta pasta.

**`app.ts`** _(35 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`index.ts`** _(288 linhas)_
Arquivo INDEX — ponto de entrada da pasta, exporta tudo que esta dentro.

---

### 📁 `artifacts/code-editor/.replit-artifact/`
> Pasta '.replit-artifact' — agrupamento de arquivos relacionados.

**`artifact.toml`** _(32 linhas)_
Arquivo TOML — parte do projeto.

---

### 📁 `artifacts/code-editor/public/`
> Arquivos estaticos: imagens, icones, fontes, arquivos publicos.

**`favicon.svg`** _(17 linhas)_
Imagem vetorial (icone ou ilustracao que nao perde qualidade ao ampliar).

**`guia-completo-apk.md`** _(949 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`manifest.json`** _(61 linhas)_
Manifesto do PWA — define nome, icone e configuracoes para instalar o app no celular.

**`sw.js`** _(176 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `artifacts/code-editor/src/`
> Codigo-fonte principal do projeto. Nao apague esta pasta.

**`App.tsx`** _(210 linhas)_
Componente RAIZ do frontend — e o pai de todos os outros componentes. Aqui ficam as rotas principais.

**`index.css`** _(167 linhas)_
Arquivo de estilos visuais — cores, tamanhos, fontes, espacamentos da interface.

**`main.tsx`** _(6 linhas)_
Ponto de entrada do React — monta o componente App na pagina HTML.

---

### 📁 `lib/api-client-react/src/`
> Codigo-fonte principal do projeto. Nao apague esta pasta.

**`custom-fetch.ts`** _(372 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`index.ts`** _(5 linhas)_
Arquivo INDEX — ponto de entrada da pasta, exporta tudo que esta dentro.

---

### 📁 `lib/api-zod/src/`
> Codigo-fonte principal do projeto. Nao apague esta pasta.

**`index.ts`** _(3 linhas)_
Arquivo INDEX — ponto de entrada da pasta, exporta tudo que esta dentro.

---

### 📁 `lib/db/src/`
> Codigo-fonte principal do projeto. Nao apague esta pasta.

**`index.ts`** _(17 linhas)_
Arquivo INDEX — ponto de entrada da pasta, exporta tudo que esta dentro.

---

### 📁 `artifacts/api-server/src/lib/`
> Funcoes auxiliares reutilizaveis em varios lugares do projeto.

**`logger.ts`** _(21 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `artifacts/api-server/src/routes/`
> Definicao das URLs e navegacao do app.

**`ai-chat.ts`** _(137 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`ai-forward.ts`** _(156 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`config.ts`** _(27 linhas)_
Arquivo de CONSTANTES/CONFIGURACAO — valores fixos usados em varios lugares do projeto.

**`db.ts`** _(362 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`drive.ts`** _(108 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`exec.ts`** _(307 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`github.ts`** _(107 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`health.ts`** _(12 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`index.ts`** _(37 linhas)_
Arquivo INDEX — ponto de entrada da pasta, exporta tudo que esta dentro.

**`legal-ai.ts`** _(328 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`proxy.ts`** _(62 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`search.ts`** _(63 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`twa.ts`** _(487 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`upload.ts`** _(77 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`voice.ts`** _(88 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`workspace.ts`** _(318 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `artifacts/code-editor/src/components/`
> Pecas visuais reutilizaveis da interface (botoes, cards, formularios...).

**`AIChat.tsx`** _(2277 linhas)_
Componente de CHAT/MENSAGENS — interface de conversa em tempo real.

**`AssistenteJuridico.tsx`** _(1286 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`CampoLivre.tsx`** _(740 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`CodeEditor.tsx`** _(154 linhas)_
Componente EDITOR — area de edicao de texto, codigo ou conteudo rico.

**`CombinarApps.tsx`** _(277 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`DriveBackupPanel.tsx`** _(200 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`EditorLayout.tsx`** _(2783 linhas)_
Componente de LAYOUT — define a estrutura visual da pagina (cabecalho, sidebar, rodape). Envolve outros componentes.

**`FileTree.tsx`** _(400 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`GitHubPanel.tsx`** _(632 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`Manual.tsx`** _(1655 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`PackageSearch.tsx`** _(415 linhas)_
Componente de BUSCA — campo e logica para filtrar/encontrar conteudo.

**`Preview.tsx`** _(496 linhas)_
Componente de PAGINA/TELA — representa uma tela completa navegavel no app.

**`QuickPrompt.tsx`** _(274 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`RealTerminal.tsx`** _(724 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`StreamTerminal.tsx`** _(539 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`SystemStatusPanel.tsx`** _(351 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`TemplateSelector.tsx`** _(501 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`Terminal.tsx`** _(1511 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`VoiceCard.tsx`** _(427 linhas)_
Componente CARD (cartao) — exibe uma informacao em um bloco visual com borda e sombra. Muito usado para listas de items.

**`VoiceMode.tsx`** _(277 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`WebContainerTerminal.tsx`** _(323 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

---

### 📁 `artifacts/code-editor/src/hooks/`
> Hooks React customizados — logica reutilizavel de estado e efeitos.

**`use-mobile.tsx`** _(20 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`use-toast.ts`** _(192 linhas)_
HOOK React personalizado para gerenciar estado/comportamento de '-toast'.

---

### 📁 `artifacts/code-editor/src/lib/`
> Funcoes auxiliares reutilizaveis em varios lugares do projeto.

**`ai-service.ts`** _(392 linhas)_
Arquivo de SERVICO/API — funcoes para comunicar com o servidor ou API externa.

**`github-service.ts`** _(197 linhas)_
Arquivo de SERVICO/API — funcoes para comunicar com o servidor ou API externa.

**`projects.ts`** _(206 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`store.ts`** _(38 linhas)_
STORE de estado — gerencia o estado global do app (dados compartilhados entre telas).

**`templates.ts`** _(4532 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`tts-service.ts`** _(312 linhas)_
Arquivo de SERVICO/API — funcoes para comunicar com o servidor ou API externa.

**`utils.ts`** _(7 linhas)_
Funcoes UTILITARIAS — ferramentas reutilizaveis de uso geral no projeto.

**`virtual-fs.ts`** _(200 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`zip-service.ts`** _(163 linhas)_
Arquivo de SERVICO/API — funcoes para comunicar com o servidor ou API externa.

---

### 📁 `lib/api-client-react/src/generated/`
> Pasta 'generated' — agrupamento de arquivos relacionados.

**`api.schemas.ts`** _(11 linhas)_
Arquivo de SERVICO/API — funcoes para comunicar com o servidor ou API externa.

**`api.ts`** _(102 linhas)_
Arquivo de SERVICO/API — funcoes para comunicar com o servidor ou API externa.

---

### 📁 `lib/api-zod/src/generated/`
> Pasta 'generated' — agrupamento de arquivos relacionados.

**`api.ts`** _(17 linhas)_
Arquivo de SERVICO/API — funcoes para comunicar com o servidor ou API externa.

---

### 📁 `lib/db/src/schema/`
> Pasta 'schema' — agrupamento de arquivos relacionados.

**`index.ts`** _(20 linhas)_
Arquivo INDEX — ponto de entrada da pasta, exporta tudo que esta dentro.

---

### 📁 `artifacts/code-editor/src/components/ui/`
> Componentes de UI (interface) basicos e genericos.

**`accordion.tsx`** _(56 linhas)_
Componente ACCORDION — secoes que abrem/fecham ao clicar, economizando espaco na tela.

**`alert-dialog.tsx`** _(140 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`alert.tsx`** _(60 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`aspect-ratio.tsx`** _(6 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`avatar.tsx`** _(51 linhas)_
Componente AVATAR — foto ou iniciais do usuario em formato circular.

**`badge.tsx`** _(44 linhas)_
Componente BADGE (etiqueta) — pequeno indicador com numero ou status (ex: '3 novas mensagens').

**`breadcrumb.tsx`** _(116 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`button-group.tsx`** _(84 linhas)_
Componente de BOTAO — elemento clicavel reutilizavel com estilo padrao do projeto.

**`button.tsx`** _(66 linhas)_
Componente de BOTAO — elemento clicavel reutilizavel com estilo padrao do projeto.

**`calendar.tsx`** _(214 linhas)_
Componente CALENDARIO/AGENDA — visualizacao e selecao de datas e eventos.

**`card.tsx`** _(77 linhas)_
Componente CARD (cartao) — exibe uma informacao em um bloco visual com borda e sombra. Muito usado para listas de items.

**`carousel.tsx`** _(261 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`chart.tsx`** _(368 linhas)_
Componente de GRAFICO — visualizacao de dados em forma de grafico (barras, linhas, pizza...).

**`checkbox.tsx`** _(29 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`collapsible.tsx`** _(12 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`command.tsx`** _(154 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`context-menu.tsx`** _(199 linhas)_
CONTEXT do React — mecanismo para compartilhar dados entre componentes sem passar por props.

**`dialog.tsx`** _(121 linhas)_
Componente DIALOG — caixa de dialogo que exige resposta do usuario (confirmar, cancelar...).

**`drawer.tsx`** _(117 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`dropdown-menu.tsx`** _(202 linhas)_
Componente de MENU/DROPDOWN — lista de opcoes que aparece ao clicar em um botao.

**`empty.tsx`** _(105 linhas)_
Componente de ESTADO VAZIO — exibido quando nao ha dados para mostrar (ex: 'Nenhum resultado encontrado').

**`field.tsx`** _(245 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`form.tsx`** _(177 linhas)_
Componente de FORMULARIO — campos de entrada de dados (texto, selecao, etc.) com validacao.

**`hover-card.tsx`** _(28 linhas)_
Componente CARD (cartao) — exibe uma informacao em um bloco visual com borda e sombra. Muito usado para listas de items.

**`input-group.tsx`** _(169 linhas)_
Componente de CAMPO DE ENTRADA — elemento de input com estilo personalizado.

**`input-otp.tsx`** _(70 linhas)_
Componente de CAMPO DE ENTRADA — elemento de input com estilo personalizado.

**`input.tsx`** _(23 linhas)_
Componente de CAMPO DE ENTRADA — elemento de input com estilo personalizado.

**`item.tsx`** _(194 linhas)_
Componente de ITEM — representa um elemento individual dentro de uma lista ou colecao.

**`kbd.tsx`** _(29 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`label.tsx`** _(27 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`menubar.tsx`** _(255 linhas)_
Componente de MENU/DROPDOWN — lista de opcoes que aparece ao clicar em um botao.

**`navigation-menu.tsx`** _(129 linhas)_
Componente de NAVEGACAO/CABECALHO — barra superior com logo, menu e links de navegacao.

**`pagination.tsx`** _(118 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`popover.tsx`** _(32 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`progress.tsx`** _(29 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`radio-group.tsx`** _(43 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`resizable.tsx`** _(46 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`scroll-area.tsx`** _(47 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`select.tsx`** _(160 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`separator.tsx`** _(30 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`sheet.tsx`** _(141 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`sidebar.tsx`** _(728 linhas)_
Componente de BARRA LATERAL — menu ou painel que aparece na lateral da tela.

**`skeleton.tsx`** _(16 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`slider.tsx`** _(27 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`sonner.tsx`** _(32 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`spinner.tsx`** _(17 linhas)_
Componente de CARREGAMENTO — animacao visual que aparece enquanto dados estao sendo buscados.

**`switch.tsx`** _(28 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`table.tsx`** _(121 linhas)_
Componente de TABELA — exibe dados em linhas e colunas.

**`tabs.tsx`** _(54 linhas)_
Componente de ABAS — permite alternar entre diferentes secoes de conteudo com clique.

**`textarea.tsx`** _(23 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`toast.tsx`** _(128 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`toaster.tsx`** _(34 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`toggle-group.tsx`** _(62 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`toggle.tsx`** _(44 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`tooltip.tsx`** _(33 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

---

### 📁 `lib/api-zod/src/generated/types/`
> Definicoes de tipos TypeScript — contratos de dados.

**`healthStatus.ts`** _(12 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`index.ts`** _(10 linhas)_
Arquivo INDEX — ponto de entrada da pasta, exporta tudo que esta dentro.

---

## CONTEXTO PARA IA (copie e cole para continuar o projeto)

> Use este bloco para explicar o projeto para qualquer IA ou desenvolvedor:

```
Projeto: sk-editor-source
Tipo: Aplicacao Web Frontend (React)
Stack: React, TypeScript
Arquivos: 149 | Linhas: ~35.063
Rotas API: 72 endpoint(s) detectado(s)
Variaveis de ambiente necessarias: LOG_LEVEL, DATABASE_URL, AI_INTEGRATIONS_OPENAI_BASE_URL, AI_INTEGRATIONS_OPENAI_API_KEY, PORT, ALLOWED_ORIGINS, JWT_SECRET, JWT_EXPIRES_IN, GROQ_API_KEY, OPENAI_API_KEY, GEMINI_API_KEY, ANTHROPIC_API_KEY, XAI_API_KEY, OPENROUTER_API_KEY, PERPLEXITY_API_KEY, TELEGRAM_TOKEN, BASE_PATH, REPL_ID

Estrutura principal:
  SK-EDITOR-README.md
  artifacts/api-server/.replit-artifact/artifact.toml
  artifacts/api-server/build.mjs
  artifacts/api-server/package.json
  artifacts/api-server/pty_helper.c
  artifacts/api-server/src/app.ts
  artifacts/api-server/src/index.ts
  artifacts/api-server/src/lib/logger.ts
  artifacts/api-server/src/routes/ai-chat.ts
  artifacts/api-server/src/routes/ai-forward.ts
  artifacts/api-server/src/routes/config.ts
  artifacts/api-server/src/routes/db.ts
  artifacts/api-server/src/routes/drive.ts
  artifacts/api-server/src/routes/exec.ts
  artifacts/api-server/src/routes/github.ts
  artifacts/api-server/src/routes/health.ts
  artifacts/api-server/src/routes/index.ts
  artifacts/api-server/src/routes/legal-ai.ts
  artifacts/api-server/src/routes/proxy.ts
  artifacts/api-server/src/routes/search.ts
  artifacts/api-server/src/routes/twa.ts
  artifacts/api-server/src/routes/upload.ts
  artifacts/api-server/src/routes/voice.ts
  artifacts/api-server/src/routes/workspace.ts
  artifacts/api-server/tsconfig.json
  artifacts/code-editor/.replit-artifact/artifact.toml
  artifacts/code-editor/SYSTEM_DOCS.md
  artifacts/code-editor/components.json
  artifacts/code-editor/index.html
  artifacts/code-editor/package.json
  artifacts/code-editor/public/favicon.svg
  artifacts/code-editor/public/guia-completo-apk.md
  artifacts/code-editor/public/manifest.json
  artifacts/code-editor/public/sw.js
  artifacts/code-editor/src/App.tsx
  artifacts/code-editor/src/components/AIChat.tsx
  artifacts/code-editor/src/components/AssistenteJuridico.tsx
  artifacts/code-editor/src/components/CampoLivre.tsx
  artifacts/code-editor/src/components/CodeEditor.tsx
  artifacts/code-editor/src/components/CombinarApps.tsx
  artifacts/code-editor/src/components/DriveBackupPanel.tsx
  artifacts/code-editor/src/components/EditorLayout.tsx
  artifacts/code-editor/src/components/FileTree.tsx
  artifacts/code-editor/src/components/GitHubPanel.tsx
  artifacts/code-editor/src/components/Manual.tsx
  artifacts/code-editor/src/components/PackageSearch.tsx
  artifacts/code-editor/src/components/Preview.tsx
  artifacts/code-editor/src/components/QuickPrompt.tsx
  artifacts/code-editor/src/components/RealTerminal.tsx
  artifacts/code-editor/src/components/StreamTerminal.tsx
  artifacts/code-editor/src/components/SystemStatusPanel.tsx
  artifacts/code-editor/src/components/TemplateSelector.tsx
  artifacts/code-editor/src/components/Terminal.tsx
  artifacts/code-editor/src/components/VoiceCard.tsx
  artifacts/code-editor/src/components/VoiceMode.tsx
  artifacts/code-editor/src/components/WebContainerTerminal.tsx
  artifacts/code-editor/src/components/ui/accordion.tsx
  artifacts/code-editor/src/components/ui/alert-dialog.tsx
  artifacts/code-editor/src/components/ui/alert.tsx
  artifacts/code-editor/src/components/ui/aspect-ratio.tsx
  artifacts/code-editor/src/components/ui/avatar.tsx
  artifacts/code-editor/src/components/ui/badge.tsx
  artifacts/code-editor/src/components/ui/breadcrumb.tsx
  artifacts/code-editor/src/components/ui/button-group.tsx
  artifacts/code-editor/src/components/ui/button.tsx
  artifacts/code-editor/src/components/ui/calendar.tsx
  artifacts/code-editor/src/components/ui/card.tsx
  artifacts/code-editor/src/components/ui/carousel.tsx
  artifacts/code-editor/src/components/ui/chart.tsx
  artifacts/code-editor/src/components/ui/checkbox.tsx
  artifacts/code-editor/src/components/ui/collapsible.tsx
  artifacts/code-editor/src/components/ui/command.tsx
  artifacts/code-editor/src/components/ui/context-menu.tsx
  artifacts/code-editor/src/components/ui/dialog.tsx
  artifacts/code-editor/src/components/ui/drawer.tsx
  artifacts/code-editor/src/components/ui/dropdown-menu.tsx
  artifacts/code-editor/src/components/ui/empty.tsx
  artifacts/code-editor/src/components/ui/field.tsx
  artifacts/code-editor/src/components/ui/form.tsx
  artifacts/code-editor/src/components/ui/hover-card.tsx
  artifacts/code-editor/src/components/ui/input-group.tsx
  artifacts/code-editor/src/components/ui/input-otp.tsx
  artifacts/code-editor/src/components/ui/input.tsx
  artifacts/code-editor/src/components/ui/item.tsx
  artifacts/code-editor/src/components/ui/kbd.tsx
  artifacts/code-editor/src/components/ui/label.tsx
  artifacts/code-editor/src/components/ui/menubar.tsx
  artifacts/code-editor/src/components/ui/navigation-menu.tsx
  artifacts/code-editor/src/components/ui/pagination.tsx
  artifacts/code-editor/src/components/ui/popover.tsx
  artifacts/code-editor/src/components/ui/progress.tsx
  artifacts/code-editor/src/components/ui/radio-group.tsx
  artifacts/code-editor/src/components/ui/resizable.tsx
  artifacts/code-editor/src/components/ui/scroll-area.tsx
  artifacts/code-editor/src/components/ui/select.tsx
  artifacts/code-editor/src/components/ui/separator.tsx
  artifacts/code-editor/src/components/ui/sheet.tsx
  artifacts/code-editor/src/components/ui/sidebar.tsx
  artifacts/code-editor/src/components/ui/skeleton.tsx
  artifacts/code-editor/src/components/ui/slider.tsx
  artifacts/code-editor/src/components/ui/sonner.tsx
  artifacts/code-editor/src/components/ui/spinner.tsx
  artifacts/code-editor/src/components/ui/switch.tsx
  artifacts/code-editor/src/components/ui/table.tsx
  artifacts/code-editor/src/components/ui/tabs.tsx
  artifacts/code-editor/src/components/ui/textarea.tsx
  artifacts/code-editor/src/components/ui/toast.tsx
  artifacts/code-editor/src/components/ui/toaster.tsx
  artifacts/code-editor/src/components/ui/toggle-group.tsx
  artifacts/code-editor/src/components/ui/toggle.tsx
  artifacts/code-editor/src/components/ui/tooltip.tsx
  artifacts/code-editor/src/hooks/use-mobile.tsx
  artifacts/code-editor/src/hooks/use-toast.ts
  artifacts/code-editor/src/index.css
  artifacts/code-editor/src/lib/ai-service.ts
  artifacts/code-editor/src/lib/github-service.ts
  artifacts/code-editor/src/lib/projects.ts
  artifacts/code-editor/src/lib/store.ts
  artifacts/code-editor/src/lib/templates.ts
  artifacts/code-editor/src/lib/tts-service.ts
  artifacts/code-editor/src/lib/utils.ts
  artifacts/code-editor/src/lib/virtual-fs.ts
  artifacts/code-editor/src/lib/zip-service.ts
  artifacts/code-editor/src/main.tsx
  artifacts/code-editor/tsconfig.json
  artifacts/code-editor/vite.config.ts
  lib/api-client-react/package.json
  lib/api-client-react/src/custom-fetch.ts
  lib/api-client-react/src/generated/api.schemas.ts
  lib/api-client-react/src/generated/api.ts
  lib/api-client-react/src/index.ts
  lib/api-client-react/tsconfig.json
  lib/api-spec/openapi.yaml
  lib/api-spec/orval.config.ts
  lib/api-spec/package.json
  lib/api-zod/package.json
  lib/api-zod/src/generated/api.ts
  lib/api-zod/src/generated/types/healthStatus.ts
  lib/api-zod/src/generated/types/index.ts
  lib/api-zod/src/index.ts
  lib/api-zod/tsconfig.json
  lib/db/drizzle.config.ts
  lib/db/package.json
  lib/db/src/index.ts
  lib/db/src/schema/index.ts
  lib/db/tsconfig.json
  package.json
  pnpm-workspace.yaml
  replit.md
```

---

*Plano gerado pelo SK Code Editor — 12/07/2026, 13:30:44*