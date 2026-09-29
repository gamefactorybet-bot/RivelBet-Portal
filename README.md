# RivelBet — Portal del jugador

Sitio del jugador. La caja, la API y el SQL están en `RivelBet-Panel`.
Este repositorio no incluye la carpeta `api`.

## Build

```bash
npm install
npm run build:portal
```

## Variables del deploy

Solo las públicas. No van la service role, el secreto de los tokens, ni las claves de Cloudinary o Telegram.

```
VITE_APP_MODE=portal
VITE_API_BASE=https://url-del-panel
VITE_SUPABASE_URL=
VITE_SUPABASE_ANON_KEY=
VITE_CURRENCY_CODE=PYG
VITE_APP_NAME=RivelBet
```

`VITE_API_BASE` es el origen del panel, sin barra final. El portal llama a rutas como `/api/player-sesion` contra esa URL.
