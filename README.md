This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.

---

## Passo a Passo do Setup do Projeto

```ts
npx create-next-app@14.2.5 fsw-barber // Cria projeto Next

npm install prisma@5.17.0 --save-dev // Instala Prisma

npx prisma init --datasource-provider postgresql // Cria pasta do prisma com o schema

// Configurar o .env com a conexão do banco de dados PostgreSQL

// Criar os modelos no schema.prisma

npx prisma format // Formata o schema, se necessário

npx prisma migrate dev --name init_db // Roda a migration

// Criar o seed

// Configurar o package.json para rodar o seed

npm install -D ts-node@10.9.2

npx prisma db seed // Roda o seed
```
