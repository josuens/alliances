<p align="center">
  <img src="https://i.imgur.com/5VcFYfp.png" alt="Alliances Logo" width="96">
</p>

<h1 align="center">Alliances — Discord Partnerships Bot</h1>

<p align="center">
  <a href="https://discord.com/api/oauth2/authorize?client_id=1410651859936608326&permissions=8&scope=bot%20applications.commands">
    <img alt="Invite the bot" src="https://img.shields.io/badge/INVITE%20BOT-5865F2?style=for-the-badge&logo=discord&logoColor=white&labelColor=1f2335">
  </a>
  <a href="https://discord.gg/xV4788y5pD">
    <img alt="Support server" src="https://img.shields.io/badge/SUPPORT%20SERVER-4461f2?style=for-the-badge&logo=discord&logoColor=white&labelColor=1f2335">
  </a>
  <a href="https://github.com/josuens/alliances/stargazers">
    <img alt="Star this repo" src="https://img.shields.io/github/stars/josuens/alliances?style=for-the-badge&label=STAR&logo=github&color=ffd83d&labelColor=1f2335">
  </a>
</p>

<p align="center">
  🇺🇸 Manage server partnerships with templates, verification codes, modern embeds, and smart controls — all via slash commands.
</p>

<p align="center">
  <img src="https://i.imgur.com/TEyCJbB.png" alt="Alliances — Preview Banner" width="960">
</p>

---

<details>
  <summary><b>English</b> — Overview, Highlights & Commands</summary>

### Overview
**Alliances** is a modern Discord bot to run **server partnerships** the right way: propose alliances, verify with secure codes, approve/decline with buttons, and publish sleek embeds using **templates** — all through **intuitive slash commands**.

### Highlights
- 🔗 **End-to-end alliance flow** — propose → verify (one-time code) → accept or reject.
- 📝 **Embeds & templates** — public/private templates with Markdown and dynamic vars:
  `GUILD_NAME`, `GUILD_ID`, `GUILD_ICON`, `MEMBER_COUNT`, `PARTNER_ID`, `CREATOR`, `CODE`.
- 🧭 **Multi-guild & multi-user** — role-based control and permission checks.
- 🛡️ **Safety controls** — server blocklist, intake toggle, global availability.
- 🌍 **Bilingual** — English & Spanish for all messages. Switch anytime with `/lang`.
- 💎 **VIP tier** — higher limits (alliances/templates) and shorter send cooldown.
- 📣 **Modern, branded embeds** — unified footer `ALLIANCE.TOP`, timestamp, emojis.
- 🔔 **Smart notifications** — admin channel for invites/updates; publish channel for partners.

### Commands (English names, localized descriptions)

**General**
- `/help` — Show help and quick guidance  
- `/lang code:<en|es>` — Switch bot language for messages

**Setup**
- `/setup channel type:<admin|publish> channel:<#channel>` — Set admin & publish channels  
- `/setup role role:<@role>` — Choose who can manage alliances

**Templates (per guild)**
- `/template create` — Create a template via modal (name, title, description, optional image)  
- `/template list` — View templates  
- `/template edit name:<TemplateName>` — Update a template  
- `/template delete name:<TemplateName>` — Remove a template  
*Default limit: 3 templates per guild (VIP: higher).*

**Alliances**
- `/alliance propose target_guild_id:<ID>` — Propose a new alliance  
- `/alliance list` — List current alliances  
- `/alliance remove target_guild_id:<ID>` — Remove an alliance (both directions)  
*Default limit: 3 alliances per guild (VIP: higher). Requires the bot installed & configured on **both** servers.*

**Sending Templates**
- `/send template target_guild_id:<ID> template:<TemplateName>` — Publish a template to an allied server  
  • Cooldown per alliance: every **5 days** (VIP: **24h**)  
  • Requires at least **1 template**

**Availability & Discovery**
- `/toggle allow:<true|false>` — Allow/block new requests (also blocks acceptance)  
- `/public set enable:<true|false>` — Join/leave the global “public” list  
- `/public list` — Discover public servers

**VIP**
- `/vip enable:<true|false>` — Mark current guild as VIP (owner only)

**Like it?** ⭐ Star the repo → https://github.com/josuens/alliances
</details>

---

<details>
  <summary><b>Español</b> — Descripción, Destacados y Comandos</summary>

### Descripción
**Alliances** permite a las comunidades gestionar **alianzas entre servidores** como debe ser: propone alianzas, verifica con **códigos de seguridad**, aprueba/rechaza con botones y publica **embeds** elegantes con **plantillas** — todo mediante **comandos slash**.

### Destacados
- 🔗 **Flujo completo de alianzas** — propuesta → verificación (código único) → aceptar o rechazar.
- 📝 **Embeds y plantillas** — plantillas públicas/privadas con Markdown y variables:
  `GUILD_NAME`, `GUILD_ID`, `GUILD_ICON`, `MEMBER_COUNT`, `PARTNER_ID`, `CREATOR`, `CODE`.
- 🧭 **Multi-servidor & multi-usuario** — control por roles y validación de permisos.
- 🛡️ **Controles de seguridad** — lista de bloqueo, toggle de recepción, disponibilidad pública.
- 🌍 **Bilingüe** — inglés y español para todos los mensajes. Cambia con `/lang`.
- 💎 **Nivel VIP** — límites superiores (alianzas/plantillas) y cooldown más corto.
- 📣 **Embeds modernos y de marca** — footer unificado `ALLIANCE.TOP`, timestamp, emojis.
- 🔔 **Notificaciones claras** — canal de admin para invitaciones/actualizaciones; canal de publicaciones para partners.

### Comandos (nombres en inglés, descripciones localizadas)

**General**
- `/help` — Ver ayuda y guía rápida  
- `/lang code:<en|es>` — Cambiar el idioma de los mensajes

**Configuración**
- `/setup channel type:<admin|publish> channel:<#channel>` — Definir canales de admin y publicaciones  
- `/setup role role:<@role>` — Elegir quién gestiona las alianzas

**Plantillas (por servidor)**
- `/template create` — Crear plantilla con modal (nombre, título, descripción, imagen opcional)  
- `/template list` — Ver plantillas  
- `/template edit name:<TemplateName>` — Actualizar una plantilla  
- `/template delete name:<TemplateName>` — Eliminar una plantilla  
*Límite por defecto: 3 plantillas por servidor (VIP: más).*

**Alianzas**
- `/alliance propose target_guild_id:<ID>` — Proponer una nueva alianza  
- `/alliance list` — Listar alianzas actuales  
- `/alliance remove target_guild_id:<ID>` — Eliminar una alianza (en ambos sentidos)  
*Límite por defecto: 3 alianzas por servidor (VIP: más). Requiere el bot instalado y configurado en **ambos** servidores.*

**Envío de plantillas**
- `/send template target_guild_id:<ID> template:<TemplateName>` — Publicar una plantilla al servidor aliado  
  • Cooldown por alianza: cada **5 días** (VIP: **24h**)  
  • Requiere mínimo **1 plantilla**

**Disponibilidad & Descubrimiento**
- `/toggle allow:<true|false>` — Permitir/bloquear nuevas solicitudes (también bloquea aceptar)  
- `/public set enable:<true|false>` — Activar/desactivar visibilidad pública  
- `/public list` — Ver servidores públicos

**VIP**
- `/vip enable:<true|false>` — Marcar este servidor como VIP (solo dueño)

**¿Te gusta?** ⭐ Dale una estrella → https://github.com/josuens/alliances
</details>
