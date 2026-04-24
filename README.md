# FSW Barber

Plataforma de agendamento de serviços para barbearias.

- **Projeto online**: https://fsw-barber-omega.vercel.app/

## Tecnologias utilizadas

- **Next.js 14 (App Router)**: framework React com SSR/SSG, rotas e Server Components.
- **React 18**: construção da interface e composição de componentes.
- **TypeScript**: tipagem estática e melhor DX.
- **Tailwind CSS**: estilização utilitária e responsiva.
- **Radix UI**: componentes acessíveis (ex.: `Dialog`, `Avatar`, `Label`, `Slot`).
- **Prisma**: ORM e geração do cliente de acesso ao banco.
- **PostgreSQL**: banco de dados (configurado via `DATABASE_URL` no Prisma).
- **NextAuth.js**: autenticação (com provider do Google) e persistência via Prisma Adapter.
- **React Hook Form + Zod**: formulários e validação de dados.
- **date-fns**: manipulação e formatação de datas.
- **react-day-picker**: seleção de datas/calendário.
- **next-themes**: suporte a tema (ex.: dark mode).
- **lucide-react**: ícones.
- **sonner**: toasts/feedbacks de UI.
- **ESLint + Prettier (+ plugin Tailwind)**: padronização e formatação do código.
- **Husky + lint-staged**: hooks de Git para manter qualidade antes de commits.

## Como rodar o projeto localmente

Instale as dependências:

```bash
npm install
```

Gere o Prisma Client e rode as migrations (ajuste a `DATABASE_URL` no `.env` antes):

```bash
npx prisma generate
npx prisma migrate dev
```

Rode o servidor de desenvolvimento:

```bash
npm run dev
```

Abra `http://localhost:3000` no navegador.
