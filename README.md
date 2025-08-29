# Render Web Service - Redirección a B@nreservas

Proyecto listo para desplegar como **Web Service** en Render.

## Estructura
- `server.js`: servidor Express que sirve `/public`
- `package.json`: scripts y dependencias
- `public/index.html`: pantalla con loader, mensaje y contador (5s) que redirige a B@nreservas. También incluye un botón "Ir ahora".

## Deploy en Render
1. Sube este repo a GitHub.
2. En Render, crea **New + → Web Service** (Runtime: Node).
3. Build Command: *(vacío)* o `npm install`
4. Start Command: `npm start`
5. Deploy.

## Cambiar destino o tiempo
- Edita `public/index.html`:
  - URL destino: `const target = "https://bancanet.bnreservas.com/";`
  - Segundos: cambia `let secs = 5;`
