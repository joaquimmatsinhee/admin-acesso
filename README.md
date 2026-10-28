# Painel Admin — Node + Neon + Upload de arquivo

Cadastre vídeos **pelo dispositivo** (celular/computador), não por URL.

## Como funciona
1. Você escolhe o arquivo de vídeo no formulário
2. O servidor envia para o storage S3 (Neon)
3. A URL gerada é salva na tabela `videos`

## Render
- Build: `npm install`
- Start: `npm start`
- Env opcional:
  - `DATABASE_URL`
  - `AWS_ENDPOINT_URL_S3`
  - `AWS_ACCESS_KEY_ID`
  - `AWS_SECRET_ACCESS_KEY`
  - `AWS_REGION`
  - `S3_BUCKET`

## Limite
Upload até **500 MB** por arquivo (ajuste no Render se o proxy cortar antes).

## API
- `POST /api/upload` (multipart: `file`, `kind=video|thumb`)
- CRUD `/api/videos`
- Telegram `/api/settings/telegram`
