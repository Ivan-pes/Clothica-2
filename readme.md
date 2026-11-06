# Clothica

Онлайн-магазин одягу. Фінальний командний проєкт GoIT

backend/ API: Node.js, Express, MongoDB
frontend/ Сайт: Next.js

````

## Запуск бекенду

```bash
cd backend
npm install
cp .env.template .env
npm run dev
````

## Запуск фронтенду

```bash
cd frontend
npm install
cp .env.template .env.local
npm run dev
```

Запити до бекенду йдуть через `app/api` за допомогою `api` з `lib/api/api.ts`:

```ts
import { api } from "@/lib/api/api";

const { data } = await api.get("/categories");
```
