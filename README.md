# FABYP — v10.0.0

> Plugin de BetterDiscord para control avanzado de RTC, bypasses y personalización de la plataforma.

Llevo bastante tiempo trabajando en esto y la verdad es que se ha ido de las manos con la cantidad de cosas que tiene.  
Básicamente es una navaja suiza para Discord: monitorea tus conexiones de voz en tiempo real, desbloquea funciones premium, y te da control total sobre cómo se comporta el cliente.

*(Mira la carpeta `src/` para ver el vídeo del panel en funcionamiento)*

---

## Qué hace

### 🔧 WebRTC & Monitoreo
- Seguimiento en directo de IPs, candidatos ICE, servidores STUN/TURN
- Datos de paquetes y payload visibles en el panel
- Contador de tiempo en llamada
- Control total del ancho de banda y bitrate de audio/vídeo

### 📡 Calidad de Stream
- Resolución, FPS y bitrate personalizables sin límite
- Forzar stream en calidad máxima (4K, alta tasa de bits)
- Sharpen de streams para mejorar nitidez
- Preview/thumbnail de stream spoofeables
- Screenshare con audio forzado
- Soundboard, stickers, emojis desbloqueados globalmente

### 🔓 Bypasses (hay muchos, estos son los principales)
- **Nitro completo**: emojis, stickers, temas, perfiles, avatares animados, decoraciones, efectos...
- **Límites de subida**: archivos grandes sin restricción
- **SlowMode, PTT, verificación, NSFW, captcha, explorar, hubs...**
- **Límites de amigos, servidores, roles, canales, hilos, emojis, pins...**  
  *(todos configurables a valores absurdos)*
- **Anti-crash**: protección contra errores del cliente
- **Anti-AFK**: evita el estado idle
- **Ringing bypass**: desactiva el sonido de llamada entrante
- **Streamer mode bypass, DevTools forzado, consola desbloqueada**
- **Stage auto-request, invite sin límite de tiempo, foro sin moderación**

### 🛡️ Privacidad & Anti-Tracking
- Bloqueo total de telemetría (track, science, Sentry, tracing, metrics)
- Spoof de: User-Agent, OS, batería, resolución de pantalla, timezone, canvas, WebGL, audio fingerprint, fuentes, hardware concurrency, plugins del navegador, media devices...
- Bloqueo de read receipts, typing indicators, process monitor
- Do Not Track forzado
- Anti-phishing (detecta enlaces de steam/discord falsos en mensajes)

### 🏷️ Spoofs de Perfil
- Badge de staff, Nitro, early supporter, active developer, bug hunter, HypeSquad
- Bot tag falso, admin shield falso
- Boost local spoof
- Rich Presence personalizable (nombre, detalles, estado, imágenes, botones)
- Impersonation local de IDs

### 📝 Logging
- Logger de mensajes borrados y editados (almacena en caché)
- Notificaciones toast cuando alguien borra un mensaje con mentions
- Anti ghost-ping

### 🎨 Personalización
- Temas forzados, high contrast, modo compacto
- Inyección de fuentes, desbloqueo de temas de cliente
- Banner, color de perfil, avatar animado forzados
- Desbloqueo de activity launcher, media gallery, clips, HUD

### ⚡ Panel Flotante
- Interfaz draggable con todos los controles
- Toggle rápido con Numpad 9
- Se puede ocultar/mostrar desde cualquier parte de Discord

---

## Instalación

1. Copia `FABYP.plugin.js` a tu carpeta de plugins de BetterDiscord  
   (`%appdata%/BetterDiscord/plugins/`)
2. Actívalo desde la pestaña de plugins
3. Pulsa **Numpad 9** para abrir el panel flotante
4. Configura lo que quieras desde ahí

---

## Notas

- Algunas funciones son client-side (solo las ves tú), otras afectan a las peticiones reales
- El spoof de perfil es local, nadie más ve tus badges falsos
- El plugin usa `BdApi.Patcher` para los hooks, así que no modifica archivos del cliente
- Si algo se rompe con una actualización de Discord, suele ser cuestión de que cambien los módulos internos

---

*Hecho por **Undfe** — [github.com/undefined-name12](https://github.com/undefined-name12)*
