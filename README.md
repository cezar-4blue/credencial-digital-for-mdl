# Workshop Credencial Digital — 4blue

Aplicativo web para geração de credenciais digitais personalizadas para o Workshop Máquina de Lucros.

## 🚀 Tecnologias

- React 19 + TypeScript
- Vite (Build tool)
- Tailwind CSS v4 com tema Dark + Neon Orange
- Shadcn/UI (Base UI)
- React Hook Form + Zod
- QRCode.react
- HTML-to-Image

## 🛠️ Instalação local

```bash
git clone <url-do-repositorio>
npm install
cp .env.example .env
# Edite .env e coloque sua GEMINI_API_KEY
npm run dev
```

## 🌐 Deploy no GitHub Pages

O deploy é **automático** via GitHub Actions ao fazer push na branch `main`.

### Configuração necessária (apenas uma vez):

1. Vá em **Settings > Pages** do repositório
2. Em **Source**, selecione **GitHub Actions**
3. Vá em **Settings > Secrets and variables > Actions**
4. Crie um secret chamado `GEMINI_API_KEY` com sua chave da API Gemini

Pronto! Qualquer `git push` na `main` faz o deploy automaticamente.

## 📁 Estrutura

```
├── .github/workflows/deploy.yml  ← Deploy automático
├── src/
│   ├── App.tsx
│   ├── main.tsx
│   ├── index.css
│   ├── assets/
│   │   └── logo-workshop.svg
│   ├── components/
│   │   ├── CredentialCard.tsx
│   │   ├── CredentialForm.tsx
│   │   └── ui/
│   │       ├── button.tsx
│   │       ├── input.tsx
│   │       ├── label.tsx
│   │       ├── select.tsx
│   │       └── sonner.tsx
│   └── lib/
│       └── utils.ts
├── index.html
├── vite.config.ts
└── package.json
```
