# 🌍 VPN World — Guía de Configuración Profesional

## Lo que construimos

Una miniapp de Telegram con:
- 🌎 **195 países** — todos los países del mundo
- 🔍 **Búsqueda instantánea** — encuentra cualquier país en segundos
- 🏷️ **Filtros por continente** — Europa, Asia, América, África, Oceanía
- 📊 **Dashboard de estadísticas** — países, servidores, protocolos activos
- 🖥️ **Servidores VPN por país** — con WireGuard, OpenVPN, IKEv2
- 📋 **Copia de configuración** — un toque y tienes la config lista
- 🎨 **Tema oscuro profesional** — estilo Magnus, responsive, animaciones fluidas
- 🤖 **Integración nativa Telegram** — botones, haptics, tema automático

---

## PASO 1: Crear el Bot en Telegram

1. Abre Telegram y busca **@BotFather**
2. Escribe el comando: `/newbot`
3. Ponle nombre: `VPN World` (o el que quieras)
4. Ponle username (debe terminar en `bot`): `VpnWorldBot` o `TuVPNWorldBot`
5. **Guarda el TOKEN** que te da BotFather. Es algo como:
   ```
   1234567890:ABCdefGHIjklMNOpqrsTUVwxyz
   ```
   ⚠️ Ese token es privado, no lo compartas con nadie.

---

## PASO 2: Configurar la Miniapp (Web App)

Sigue en @BotFather:

1. Escribe: `/setmenubutton`
2. Selecciona tu bot: `@VpnWorldBot`
3. Para el texto del botón pon: `🌍 Abrir VPN World`
4. Para la URL, usa la de tu despliegue (ver PASO 3)

---

## PASO 3: Desplegar la Miniapp (gratis)

Tienes 3 opciones. Elige una:

### Opción A: GitHub Pages (recomendado, 100% gratis)

```bash
# 1. Instala git si no lo tienes
# 2. Crea un repo en github.com (ej: vpn-world)
# 3. Sube los archivos:
git init
git add index.html styles.css data.js app.js
git commit -m "VPN World v1"
git remote add origin https://github.com/TU_USUARIO/vpn-world.git
git push -u origin main

# 4. En GitHub: Settings > Pages > Source: main branch > Save
# 5. Tu URL será: https://TU_USUARIO.github.io/vpn-world/
```

### Opción B: Vercel (gratis, más rápido)

1. Ve a https://vercel.com
2. Crea cuenta con GitHub
3. Importa tu repo o arrastra la carpeta
4. Te da URL tipo: `https://vpn-world.vercel.app`

### Opción C: Netlify (gratis, arrastrar y soltar)

1. Ve a https://app.netlify.com
2. Arrastra la carpeta `vpn-world-miniapp` al navegador
3. ¡Desplegado! Te da URL tipo: `https://vpn-world.netlify.app`

---

## PASO 4: Conectar la URL al Bot

Una vez desplegado, vuelve a @BotFather:

```
/setmenubutton
@VpnWorldBot
🌍 Abrir VPN World
https://TU_URL_AQUI/
```

---

## PASO 5: ¡Probar!

1. Abre Telegram
2. Busca tu bot: `@VpnWorldBot`
3. Escribe `/start`
4. Toca el botón `🌍 Abrir VPN World`
5. ¡La miniapp se abre dentro de Telegram!

---

## Estructura de archivos

```
vpn-world-miniapp/
├── index.html      ← Página principal (Telegram Web App ready)
├── styles.css      ← Tema oscuro profesional
├── data.js         ← 195 países + servidores VPN
├── app.js          ← Lógica: búsqueda, filtros, modal, copia
└── GUIA_SETUP.md   ← Esta guía
```

---

## Personalización

Para cambiar los datos de servidores (poner servidores reales), edita `data.js` en la sección `CITIES_BY_CONTINENT` y agrega servidores reales con IPs, puertos y protocolos.

Para una VPN real, necesitarás:
- Servidores VPS en cada país
- WireGuard/OpenVPN instalado en cada uno
- Panel de administración para gestionar usuarios

Eso ya es infraestructura backend — dime si quieres que te ayude con esa parte.

---

## ¿Necesitas ayuda con algo más?

- ¿Configurar un VPS real con WireGuard?
- ¿Panel de admin para gestionar servidores?
- ¿Sistema de usuarios y pagos?
- ¿App nativa para iOS/Android?

Avísame y lo construimos. 🐺
