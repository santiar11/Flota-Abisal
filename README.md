# Flota Abisal en la web (Vercel)

Esta carpeta es el juego listo para publicar como sitio estático. No necesita servidor propio, base de datos ni cuentas de Claude:
el juego en línea conecta a los dos navegadores directamente (WebRTC) y usa el servidor público y gratuito de PeerJS solo para que se encuentren.

## Publicar (elige una opción)

**A. Desde GitHub (recomendada para el equipo)**
1. Crea un repositorio y sube esta carpeta (`index.html` y `vercel.json`).
2. En vercel.com, entra con tu cuenta de GitHub → **Add New… → Project** → importa el repositorio.
3. Framework Preset: **Other**. No hace falta comando de build. Pulsa **Deploy**.
4. Cada `git push` vuelve a publicar el juego automáticamente.

**B. Desde la terminal**
```bash
cd deploy
npx vercel          # la primera vez pide iniciar sesión y crea el proyecto
npx vercel --prod   # publica en la URL definitiva
```

## Jugar en línea
1. Uno abre la web → **Jugar en línea con un amigo** → **Crear sala**.
2. Le pasa el PIN, el QR o el botón **Copiar invitación** (enlace `…/#sala-123456`).
3. El amigo abre el enlace (o escribe el PIN) → **Unirse**.

Ninguno de los dos necesita registrarse. Ambos deben usar la misma versión del juego.
