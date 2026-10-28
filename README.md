# Painel Admin — Node.js + Neon (Render)

Mesmo padrão da loja AllContent que já funciona no Render.

## Render

1. New → Web Service
2. Build: `npm install`
3. Start: `npm start`
4. (Opcional) Env: `DATABASE_URL` = connection string Neon
5. Deploy → abra a URL no PC/celular

## Local

```bash
npm install
npm start
# http://localhost:3000
```

## API

- `GET    /api/videos`
- `POST   /api/videos`
- `PUT    /api/videos/:id`
- `DELETE /api/videos/:id`
- `GET    /api/settings/telegram`
- `POST   /api/settings/telegram`
- `GET    /api/health`

Vídeos criados aqui aparecem na loja (mesmo banco Neon).
