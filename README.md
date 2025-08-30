<!--
Alliances — Discord Partnerships Bot
Compact README with collapsible sections (EN/ES). No technical setup, only features & commands.
-->

<p align="center">
  <img src="assets/banner.png" alt="Alliances — Discord Partnerships Bot" width="900">
</p>

<h1 align="center">Alliances — Discord Partnerships Bot</h1>

<p align="center">
  <a href="https://discord.com/api/oauth2/authorize?client_id=1410651859936608326&permissions=8&scope=bot%20applications.commands">
    <img src="https://img.shields.io/badge/Invite%20the%20Bot-5865F2?logo=discord&logoColor=white" alt="Invite the Bot">
  </a>
  <a href="https://discord.gg/xV4788y5pD">
    <img src="https://img.shields.io/badge/Support-Server-5865F2?logo=discord&logoColor=white" alt="Support Server">
  </a>
  <a href="https://github.com/josuens/alliances/stargazers">
    <img src="https://img.shields.io/github/stars/josuens/alliances?style=social" alt="Star this repo">
  </a>
</p>

---

<details open>
  <summary><b>English</b> — Overview, Highlights & Commands</summary>

### Overview
**Alliances** is a modern Discord bot to manage **server partnerships**: propose alliances, verify with secure codes, accept/reject with buttons, and publish polished embeds using **templates** — all via **intuitive slash commands**.

<p align="center">
  <img src="assets/demo-embed.png" alt="Alliance Proposed — Demo Embed" width="720">
</p>

### Highlights
- 🔗 **End-to-end Alliance Flow** — Propose, verify with a one-time code, accept or reject.
- 📝 **Embeds & Templates** — Public/private templates with Markdown and dynamic variables: `{GUILD_NAME} {GUILD_ID} {GUILD_ICON} {MEMBER_COUNT} {PARTNER_ID} {CREATOR} {CODE}`
- 🧭 **Multi-Guild & Multi-User** — Role-based control + permission validation.
- 🛡️ **Safety Controls** — Server blocklist, intake toggle, global availability.
- 🌍 **Bilingual** — English & Spanish. Switch anytime with `/lang`.
- 💎 **VIP Tier** — Higher limits and shorter send cooldown.
- 📣 **Branded, Modern Embeds** — Unified footer `ALLIANCE.TOP`, timestamps, emojis.
- 🔔 **Smart Notifications** — Admin channel for invites/updates; publish channel for partners.

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
> Default limit: **3 templates** per guild (VIP: higher)

**Alliances**
- `/alliance propose target_guild_id:<ID>` — Propose a new alliance  
- `/alliance list` — List current alliances  
- `/alliance remove target_guild_id:<ID>` — Remove an alliance (both directions)  
> Default limit: **3 alliances** per guild (VIP: higher)  
> Requires bot installed & configured on **both** servers

**Sending Templates**
- `/send template target_guild_id:<ID> template:<TemplateName>` — Publish a template to an allied server  
  - Cooldown per alliance: **every 5 days** (VIP: **every 24 hours**)  
  - Requires at least **1 template**

**Availability & Discovery**
- `/toggle allow:<true|false>` — Allow/block new requests (also blocks acceptance)  
- `/public set enable:<true|false>` — Join/leave global “public” list  
- `/public list` — Discover public servers

**VIP**
- `/vip enable:<true|false>` — Mark current guild as VIP (owner only)

**Love it?** ⭐ Star the repo: <https://github.com/josuens/alliances>

</details>

---

<details>
  <summary><b>Español</b> — Descripción, Destacados y Comandos</summary>

### Descripción
**Alliances** es un bot moderno para gestionar **alianzas entre servidores**: propone alianzas, verifica con **códigos de seguridad**, acepta/rechaza con botones y publica **embeds** usando **plantillas** — todo mediante **comandos slash**.

<p align="center">
  <img src="assets/demo-embed.png" alt="Alianza propuesta — Demo" width="720">
</p>

### Destacados
- 🔗 **Flujo completo de alianzas** — Propuesta, verificación por código único, aceptar o rechazar.
- 📝 **Embeds y Plantillas** — Plantillas públicas/privadas con Markdown y variables: `{GUILD_NAME} {GUILD_ID} {GUILD_ICON} {MEMBER_COUNT} {PARTNER_ID} {CREATOR} {CODE}`
- 🧭 **Multi-servidor & Multi-usuario** — Control por roles + validación de permisos.
- 🛡️ **Controles de seguridad** — Lista de bloqueo, toggle de recepción, disponibilidad pública.
- 🌍 **Bilingüe** — Inglés y español. Cambia con `/lang`.
- 💎 **Nivel VIP** — Límites superiores y cooldown más corto.
- 📣 **Embeds modernos y de marca** — Footer unificado `ALLIANCE.TOP`, timestamp, emojis.
- 🔔 **Notificaciones claras** — Canal de admin para invitaciones/actualizaciones; canal de publicaciones para partners.

### Comandos (nombres en inglés, descripciones localizadas)

**General**
- `/help` — Ver ayuda y guía rápida  
- `/lang code:<en|es>` — Cambiar el idioma de los mensajes

**Configuración**
- `/setup channel type:<admin|publish> channel:<#channel>` — Definir canales de admin y publicaciones  
- `/setup role role:<@role>` — Elegir quién gestiona las alianzas

**Plantillas (por servidor)**
- `/template create` — Crear plantilla por modal (nombre, título, descripción, imagen opcional)  
- `/template list` — Ver plantillas  
- `/template edit name:<TemplateName>` — Actualizar una plantilla  
- `/template delete name:<TemplateName>` — Eliminar una plantilla  
> Límite por defecto: **3 plantillas** por servidor (VIP: más)

**Alianzas**
- `/alliance propose target_guild_id:<ID>` — Proponer una nueva alianza  
- `/alliance list` — Listar alianzas actuales  
- `/alliance remove target_guild_id:<ID>` — Eliminar una alianza (en ambos sentidos)  
> Límite por defecto: **3 alianzas** por servidor (VIP: más)  
> Requiere el bot instalado y configurado en **ambos** servidores

**Envío de plantillas**
- `/send template target_guild_id:<ID> template:<TemplateName>` — Publicar una plantilla al servidor aliado  
  - Cooldown por alianza: **cada 5 días** (VIP: **cada 24 h**)  
  - Requiere mínimo **1 plantilla**

**Disponibilidad & Descubrimiento**
- `/toggle allow:<true|false>` — Permitir/bloquear nuevas solicitudes (también bloquea aceptar)  
- `/public set enable:<true|false>` — Activar/desactivar visibilidad pública  
- `/public list` — Ver servidores públicos

**VIP**
- `/vip enable:<true|false>` — Marcar este servidor como VIP (solo dueño)

**¿Te gusta?** ⭐ Dale una estrella: <https://github.com/josuens/alliances>

</details>
