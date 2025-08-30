<!--
Alliances — Discord Partnerships Bot
Bilingual README (EN/ES). Focused on features & commands (no technical setup).
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
    <img src="https://img.shields.io/github/stars/YOUR_USER/YOUR_REPO?style=social" alt="Star this repo">
  </a>
</p>

<p align="center">
  <b>English</b> · <a href="#español">Español</a>
</p>

---

## Overview

**Alliances** is a modern Discord bot that helps communities manage **server partnerships** in a clean, safe, and beautiful way. Propose alliances, verify with secure codes, accept/reject with buttons, and publish polished embeds using **templates** — all through **intuitive slash commands**.

<p align="center">
  <img src="assets/demo-embed.png" alt="Alliance Proposed — Demo Embed" width="720">
</p>

---

## Highlights

- 🔗 **End-to-end Alliance Flow**  
  Propose partnerships, verify with a one-time code, accept or reject via buttons, and keep both sides in sync.

- 📝 **Embeds & Templates**  
  Create public/private templates with Markdown and dynamic variables:
  ```
  {GUILD_NAME} {GUILD_ID} {GUILD_ICON} {MEMBER_COUNT}
  {PARTNER_ID} {CREATOR} {CODE}
  ```

- 🧭 **Multi-Guild & Multi-User**  
  Built for communities of any size. Choose who manages alliances with a role, plus permission checks.

- 🛡️ **Safety Controls**  
  Server blocklist, global availability, intake toggle, and code-based verification for approvals.

- 🌍 **Bilingual Out-of-the-Box**  
  English and Spanish for all bot messages. Switch anytime with `/lang`.

- 💎 **VIP Tier**  
  Higher limits (alliances/templates) and a shorter send cooldown for active networks.

- 📣 **Beautiful, Branded Embeds**  
  Modern look with emojis, unified footer `ALLIANCE.TOP`, timestamp, and your logo.

- 🔔 **Smart Notifications**  
  Admin channel for new invites and updates; publish channel for partner templates.

---

## How It Works (Simple)

1. **Set up once** with channels and a manager role.  
2. **Create a template** (name, title, description, optional image).  
3. **Propose an alliance** to another guild by ID — the other side gets a verification prompt.  
4. **Accept or reject** with buttons; accepted alliances are saved and can publish templates.  
5. **Send templates** to your partners following the cooldown rules.  
6. **Control intake** with a toggle and appear in the public directory to receive invites.

---

## Commands (English names, localized descriptions)

> All commands are slash-based; descriptions adapt to your chosen language (EN/ES).

### General
- **`/help`** — Show help and quick guidance.  
- **`/lang code:<en|es>`** — Switch bot language for messages.

### Setup
- **`/setup channel type:<admin|publish> channel:<#channel>`** — Set the admin and publish channels.  
- **`/setup role role:<@role>`** — Choose who can manage alliances.

### Templates (per guild)
- **`/template create`** — Create a template via modal (name, title, description, optional image).  
- **`/template list`** — View your templates.  
- **`/template edit name:<TemplateName>`** — Update an existing template.  
- **`/template delete name:<TemplateName>`** — Remove a template.  
> Default limit: **3 templates** per guild (VIP: higher).

### Alliances
- **`/alliance propose target_guild_id:<ID>`** — Propose a new alliance.  
- **`/alliance list`** — See current alliances and their status.  
- **`/alliance remove target_guild_id:<ID>`** — Remove an alliance in **both directions**.  
> Default limit: **3 alliances** per guild (VIP: higher).  
> Alliances work only if the bot is installed and configured on **both** servers.

### Sending Templates
- **`/send template target_guild_id:<ID> template:<TemplateName>`** — Publish a template to an allied server.  
  - Cooldown per alliance: **every 5 days** (VIP: **every 24 hours**).  
  - Requires at least **1 template** configured.

### Availability & Discovery
- **`/toggle allow:<true|false>`** — Allow or block new alliance requests (also blocks acceptance).  
- **`/public set enable:<true|false>`** — Join or leave the global “public” list (visible to other servers).  
- **`/public list`** — Discover public servers and see basic info.

### VIP
- **`/vip enable:<true|false>`** — Mark the current guild as VIP (owner-only action).

---

## Visual Language

- ✅ Success and acceptance are clear and celebratory.  
- ❌ Rejection is explicit and cleans up gracefully.  
- 🔐 Verification uses a one-time code for extra safety.  
- 📨 Admins get digestible, branded embeds with timestamps.  
- 🧭 Presence reads: **Watching `<number> servers | /help`**.

---

## Connect

- 💬 **Support server**: <a href="https://discord.gg/aws8KnzVPJ">discord.gg/aws8KnzVPJ</a>  
- 🤝 **Invite the bot**: <a href="https://discord.com/api/oauth2/authorize?client_id=1410651859936608326&permissions=8&scope=bot%20applications.commands">Add to your server</a>  
- ⭐ **Like this?** Star the repo — it helps visibility!

---

---

<a id="español"></a>

# Alliances — Bot de Alianzas para Discord

## Descripción

**Alliances** es un bot moderno para gestionar **alianzas entre servidores** de forma organizada, segura y atractiva. Crea propuestas, verifica con **código de seguridad**, acepta o rechaza con botones y publica **embeds** profesionales con **plantillas** — todo mediante **comandos slash**.

<p align="center">
  <img src="assets/demo-embed.png" alt="Alianza propuesta — Demo" width="720">
</p>

## Destacados

- 🔗 **Flujo completo de alianzas**  
  Propuesta → código de verificación → aceptar/rechazar con botones y sincronización entre servidores.

- 📝 **Embeds & Plantillas**  
  Crea plantillas públicas/privadas con Markdown y variables dinámicas:
  ```
  {GUILD_NAME} {GUILD_ID} {GUILD_ICON} {MEMBER_COUNT}
  {PARTNER_ID} {CREATOR} {CODE}
  ```

- 🧭 **Multi-servidor & Multi-usuario**  
  Pensado para comunidades de cualquier tamaño. Define quién gestiona con un rol, más validación de permisos.

- 🛡️ **Controles de seguridad**  
  Lista de bloqueo de servidores, disponibilidad global, toggle de recepción y verificación por código.

- 🌍 **Bilingüe desde el inicio**  
  Inglés y español para todos los mensajes. Cambia cuando quieras con `/lang`.

- 💎 **Nivel VIP**  
  Límites superiores (alianzas/plantillas) y cooldown más corto para envíos.

- 📣 **Embeds modernos y de marca**  
  Estilo actual con emojis, footer unificado `ALLIANCE.TOP`, timestamp y tu logo.

- 🔔 **Notificaciones claras**  
  Canal de admin para invitaciones/actualizaciones; canal de publicaciones para plantillas de partners.

---

## Cómo funciona (simple)

1. **Configura una vez** los canales y el rol gestor.  
2. **Crea una plantilla** (nombre, título, descripción e imagen opcional).  
3. **Propón una alianza** a otro servidor por ID — el destino recibe la verificación.  
4. **Acepta o rechaza** con botones; las alianzas aceptadas quedan guardadas y pueden publicar plantillas.  
5. **Envía plantillas** a tus aliados respetando el cooldown.  
6. **Controla la recepción** con el toggle y aparece en el directorio público para recibir invitaciones.

---

## Comandos (nombres en inglés, descripciones localizadas)

> Todos los comandos son tipo slash; las descripciones se adaptan a tu idioma (EN/ES).

### General
- **`/help`** — Ver ayuda y guía rápida.  
- **`/lang code:<en|es>`** — Cambiar el idioma de los mensajes.

### Configuración
- **`/setup channel type:<admin|publish> channel:<#channel>`** — Definir canales de admin y publicaciones.  
- **`/setup role role:<@role>`** — Elegir quién puede gestionar alianzas.

### Plantillas (por servidor)
- **`/template create`** — Crear plantilla con modal (nombre, título, descripción e imagen opcional).  
- **`/template list`** — Ver plantillas.  
- **`/template edit name:<TemplateName>`** — Editar una plantilla.  
- **`/template delete name:<TemplateName>`** — Eliminar una plantilla.  
> Límite por defecto: **3 plantillas** por servidor (VIP: más).

### Alianzas
- **`/alliance propose target_guild_id:<ID>`** — Proponer una nueva alianza.  
- **`/alliance list`** — Ver alianzas actuales y su estado.  
- **`/alliance remove target_guild_id:<ID>`** — Eliminar una alianza en **ambas direcciones**.  
> Límite por defecto: **3 alianzas** por servidor (VIP: más).  
> Solo funciona si el bot está instalado y configurado en **ambos** servidores.

### Envío de plantillas
- **`/send template target_guild_id:<ID> template:<TemplateName>`** — Publicar una plantilla en el servidor aliado.  
  - Cooldown por alianza: **cada 5 días** (VIP: **cada 24 h**).  
  - Requiere al menos **1 plantilla** creada.

### Disponibilidad & Descubrimiento
- **`/toggle allow:<true|false>`** — Permitir o bloquear nuevas solicitudes (también bloquea aceptación).  
- **`/public set enable:<true|false>`** — Activar/desactivar la visibilidad pública.  
- **`/public list`** — Ver servidores públicos y su información básica.

### VIP
- **`/vip enable:<true|false>`** — Marcar este servidor como VIP (solo dueño).

---

## Conecta

- 💬 **Servidor de soporte**: <a href="https://discord.gg/aws8KnzVPJ">discord.gg/aws8KnzVPJ</a>  
- 🤝 **Invitar el bot**: <a href="https://discord.com/api/oauth2/authorize?client_id=1410651859936608326&permissions=8&scope=bot%20applications.commands">Añadir a tu servidor</a>  
- ⭐ **¿Te gusta?** Dale una estrella al repo — ¡ayuda muchísimo a la visibilidad!

---
