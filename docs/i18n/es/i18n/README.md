# 🚀 OmniRoute — La Puerta Gratuito AI

### No detengas de programar. Ruteo inteligente a **modelos AI gratuitos** y de bajo costo con caída automática.

_ Tu proxy de API universal — un endpoint, 67+ proveedores, sin tiempo de
inactividad. Ahora con agentes de orquestación MCP & A2A._

** Completaciones de chat • Integraciones • Generación de imágenes • Vide •
Música • Audio • Reorganización • **búsqueda web** • Servidor MCP • Protocolo
A2A • 100% de TypeScript**

---

<div align="center">

[![Versión
npm](https://img.shields.io/npm/v/omniroute?color=cb3837&logo=npm)](https://www.npmjs.com/package/omniroute)
[![Descargas
npm](https://img.shields.io/npm/dm/omniroute?color=cb3837&logo=npm&label=npm%20downloads)](https://www.npmjs.com/package/omniroute)
[![Docker
Hub](https://img.shields.io/docker/v/diegosouzapw/omniroute?label=Docker%20Hub&logo=docker&color=2496ED)](https://hub.docker.com/r/diegosouzapw/omniroute)
[![Docker
Pulls](https://img.shields.io/docker/pulls/diegosouzapw/omniroute?logo=docker&color=2496ED&label=docker%20pulls)](https://hub.docker.com/r/diegosouzapw/omniroute)
[![Licencia](https://img.shields.io/github/license/diegosouzapw/OmniRoute)](https://github.com/diegosouzapw/OmniRoute/blob/main/LICENSE)
[![Sitio
web](https://img.shields.io/badge/Website-omniroute.online-blue?logo=google-chrome&logoColor=white)](https://omniroute.online)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-Community-25D366?logo=whatsapp&logoColor=white)](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)

[🌐 Sitio web](https://omniroute.online) • [🚀 Paso rápido](#-quick-start) • [💡
Características](#-key-features) • [📖 Documentación](#-documentation) • [💰
Precios](#-pricing-at-a-glance) • [💬
WhatsApp](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)

</div>

🌐 **Disponible en:** 🇺🇸 [Inglés](README.md) | 🇧🇷 [Português
(Brasil)](docs/i18n/pt-BR/README.md) | 🇪🇸 [Español](docs/i18n/es/README.md) | 🇫🇷
[Francés](docs/i18n/fr/README.md) | 🇮🇹 [Italiano](docs/i18n/it/README.md) | 🇷🇺
[Russo](docs/i18n/ru/README.md) | 🇨🇳 [Chino
(simplificado)](docs/i18n/zh-CN/README.md) | 🇩🇪 [Alemán](docs/i18n/de/README.md)
| 🇮🇳 [Hindi](docs/i18n/in/README.md) | 🇹🇭 [tailandés](docs/i18n/th/README.md) |
🇺🇦 [Ucraniano](docs/i18n/uk-UA/README.md) | 🇸🇦 [Árabe](docs/i18n/ar/README.md) |
🇯🇵 [japonés](docs/i18n/ja/README.md) | 🇻🇳 [vietnamita](docs/i18n/vi/README.md) |
🇧🇬 [Búlgaro](docs/i18n/bg/README.md) | 🇩🇰 [Danés](docs/i18n/da/README.md) | 🇫🇮
[Finés](docs/i18n/fi/README.md) | 🇮🇱 [Hebreo](docs/i18n/he/README.md) | 🇭🇺
[Húngaro](docs/i18n/hu/README.md) | 🇮🇩 [Indonesio](docs/i18n/id/README.md) | 🇰🇷
[coreano](docs/i18n/ko/README.md) | 🇲🇾 [malayo](docs/i18n/ms/README.md) | 🇳🇱
[holandés](docs/i18n/nl/README.md) | 🇳🇴 [noruego](docs/i18n/no/README.md) | 🇵🇹
[Portugués (Portugal)](docs/i18n/pt/README.md) | 🇷🇴
[rumano](docs/i18n/ro/README.md) | 🇵🇱 [polaco](docs/i18n/pl/README.md) | 🇸🇰
[eslovaco](docs/i18n/sk/README.md) | 🇸🇪 [sueco](docs/i18n/sv/README.md) | 🇵🇭
[filipino](docs/i18n/phi/README.md) | 🇨🇿 [checo](docs/i18n/cs/README.md)

---

## 🆕 ¿Qué hay de nuevo en v3.0.0

> ** Actualizando de v2.9.5?** — Ver el [cambio
> completo](CHANGELOG.md#300--2026-03-22-release-candidate--not-yet-merged-to-main)
> para todos los cambios.

| Área                                       | Cambio                                                                                                                                                                                                   |
| ------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🔒 **Seguridad CodeQL**                     | Se han fijado 10+ alarmas CodeQL: polynomial-redos, aleatoriedad de incertidumbre, remediación de inyección de conchas                                                                                   |
| ✅ **VALIDación de rutas**                  | Ahora todas las rutas de API se validan con esquemas Zod + `validateBody()` - CI `revisa: ruta-a-validar:t06`                                                                                            |
| 🐛 ** fugas de etiquetas omniModel**        | Las etiquetas internas <omnimodel>` ya no se propagan a los clientes en las respuestas de emisión de eventos de streaming (#585)</omnimodel>                                                             |
| 🔑 **API de claves registradas**            | Provea automáticamente claves API mediante `POST /api/v1/registered-keys` con aplicación de cuotas por proveedor/cuenta, idempotencia, almacenamiento SHA-256 y reporteo de problemas de GitHub opcional |
| 🎨 ** Iconos de proveedores**               | 130+ logos de proveedores via `@lobehub/icons` (SVG) concadena de fallback genérica a PNG                                                                                                                |
| 🔄 Sincronización de modelo Auto-AutoSync** | Scheduler y interruptor UI manual para sincronizar listas de modelo para proveedores compatibles con OpenAI integrados y personalizados                                                                  |
| 🌐 Código Abierto Zen/Go**                  | Dos nuevos proveedores de @kang-heewon mediante PR #530: tarifa gratuita + tarifa de suscripción mediante `OpencodeExecutor`                                                                             |
| 🐛 Autenticación CLI de Gemini**            | Error acciónable cuando `GEMINI_OAUTH_CLIENT_SECRET` falta en Docker (era un error Google criptográfico)                                                                                                 |
| 🐛 Configuración de OpenCode**              | `saveOpenCodeConfig()` ahora escribe correctamente TOML a `XDG_CONFIG_HOME`                                                                                                                              |
| 🐛 Superficie del modelo anclado**          | `body.model` se establece correctamente a `pinnedModel` en la protección del caché del contexto                                                                                                          |
| 🐛 Bucle de Codex/Claude**                  | `tool_result` bloques ahora se convierten a texto para detener los bucles infinitos                                                                                                                      |
| 🐛 Redireccionamiento de inicio de sesión** | El inicio de sesión ya no se congeló después de saltarse la configuración de contraseña                                                                                                                  |
| 🐛 Caminos de Windows**                     | Caminos de MSYS2/Git-Bash (/`/c/...`) se normalizan a `C:\...` automáticamente                                                                                                                           |

---

## 🖼️ Página de inicio principal

<div align="center">
  <img src="./docs/screenshots/MainOmniRoute.png" alt="OmniRoute Dashboard" width="800"/>
</div>

---

## 📸 Vista previa del portapapeles

<details>
<summary><b>Click to see dashboard screenshots</b></summary>

| Página                       | Captura de pantalla                                     |
| ---------------------------- | ------------------------------------------------------- |
| [M0M]Proveedores[M4M]        | ![Proveedores](docs/screenshots/01-providers.png)       |
| [M0M]Combinaciones[M8M]      | ![Combinaciones](docs/screenshots/02-combos.png)        |
| [M0M]Análiticas[M4M]         | ![Análiticas](docs/screenshots/03-analytics.png)        |
| [M0M]Salud[M8M]              | ![Salud](docs/screenshots/04-health.png)                |
| [M0M]Traductor[M5M]          | ![Traductor](docs/screenshots/05-translator.png)        |
| [M0M]Configuración[M10M]     | ![Configuración](docs/screenshots/06-settings.png)      |
| [M0M]Herramientas CLI[M4M]   | ![Herramientas CLI](docs/screenshots/07-cli-tools.png)  |
| [M0M]Registros de uso[M5M]   | ![Registros de Uso](docs/screenshots/08-usage.png)      |
| [M0M]Puntos de conexión[M4M] | ![Puntos de Conexión](docs/screenshots/09-endpoint.png) |

</details>

---

### 🤖 Proveedor de IA gratuito para agentes codificadores favoritos

_Conecta cualquier CLI con herramientas de código AI mediante OmniRoute — API
gateway gratuito para codificación ilimitada._

  <table>
    <tr>
      <td align="center" width="110">
        <a href="https://github.com/openclaw/openclaw">
          <img src="./public/providers/openclaw.png" alt="OpenClaw" width="48"/><br/>
          <b>OpenClaw</b>
        </a><br/>
        <sub>⭐ 205K</sub>
      </td>
      <td align="center" width="110">
        <a href="https://github.com/HKUDS/nanobot">
          <img src="./public/providers/nanobot.png" alt="NanoBot" width="48"/><br/>
          <b>NanoBot</b>
        </a><br/>
        <sub>⭐ 20.9K</sub>
      </td>
      <td align="center" width="110">
        <a href="https://github.com/sipeed/picoclaw">
          <img src="./public/providers/picoclaw.jpg" alt="PicoClaw" width="48"/><br/>
          <b>PicoClaw</b>
        </a><br/>
        <sub>⭐ 14.6K</sub>
      </td>
      <td align="center" width="110">
        <a href="https://github.com/zeroclaw-labs/zeroclaw">
          <img src="./public/providers/zeroclaw.png" alt="ZeroClaw" width="48"/><br/>
          <b>ZeroClaw</b>
        </a><br/>
        <sub>⭐ 9.9K</sub>
      </td>
      <td align="center" width="110">
        <a href="https://github.com/nearai/ironclaw">
          <img src="./public/providers/ironclaw.png" alt="IronClaw" width="48"/><br/>
          <b>IronClaw</b>
        </a><br/>
        <sub>⭐ 2.1K</sub>
      </td>
    </tr>
    <tr>
      <td align="center" width="110">
        <a href="https://github.com/anomalyco/opencode">
          <img src="./public/providers/opencode.svg" alt="OpenCode" width="48"/><br/>
          <b>OpenCode</b>
        </a><br/>
        <sub>⭐ 106K</sub>
      </td>
      <td align="center" width="110">
        <a href="https://github.com/openai/codex">
          <img src="./public/providers/codex.png" alt="Codex CLI" width="48"/><br/>
          <b>Codex CLI</b>
        </a><br/>
        <sub>⭐ 60.8K</sub>
      </td>
      <td align="center" width="110">
        <a href="https://github.com/anthropics/claude-code">
          <img src="./public/providers/claude.png" alt="Claude Code" width="48"/><br/>
          <b>Claude Code</b>
        </a><br/>
        <sub>⭐ 67.3K</sub>
      </td>
      <td align="center" width="110">
        <a href="https://github.com/google-gemini/gemini-cli">
          <img src="./public/providers/gemini-cli.png" alt="Gemini CLI" width="48"/><br/>
          <b>Gemini CLI</b>
        </a><br/>
        <sub>⭐ 94.7K</sub>
      </td>
      <td align="center" width="110">
        <a href="https://github.com/Kilo-Org/kilocode">
          <img src="./public/providers/kilocode.png" alt="Kilo Code" width="48"/><br/>
          <b>Kilo Code</b>
        </a><br/>
        <sub>⭐ 15.5K</sub>
      </td>
    </tr>
  </table>

<sub>📡 Todos los agentes conectan a través de
<code>http://localhost:20128/v1</code> o
<code>http://cloud.omniroute.online/v1</code> — una configuración, modelos
ilimitados y cuota</sub>

---

## 🤔 ¿Por qué OmniRoute?

**deténgase gastando dinero y alcanzando límites:**

- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  La cuota de suscripción vence sin utilizarse cada mes
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Limitaciones de tasa te detienen en medio de la codificación
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  APIs caras ($20-50/mes por proveedor)
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Cambios manuales entre proveedores

**OmniRoute resuelve esto:**

- ✅ **Maximice las suscripciones** - Rastrea la cuota, utilice cada bit antes de
  resetear
- ✅ **Fallo automático** - Suscripción → Llave de API → Barata → Gratuita, sin
  tiempo de inactividad
- ✅ **Cuenta múltiple** - Equilibrio de rondas entre cuentas por proveedor
- ✅ **Universal** - Funciona con Claude Code, Codex, Gemini CLI, Cursor, Cline,
  OpenClaw, cualquier herramienta CLI

---

## 📧 Soporte

> 💬 **Únete a nuestra comunidad!** [Group de
> WhatsApp](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t) — Obtién
> ayuda, comparte consejos y mantente al día

- **Sitio web**: [omniroute.online](https://omniroute.online)
- **GitHub**:
  [github.com/diegosouzapw/OmniRoute](https://github.com/diegosouzapw/OmniRoute)
- **Issues**:
  [github.com/diegosouzapw/OmniRoute/issues](https://github.com/diegosouzapw/OmniRoute/issues)
- **WhatsApp**: [Group de la
  comunidad](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)
- **Contribuir**: Consulta [CONTRIBUTING.md](CONTRIBUTING.md), abre un PR o
  selecciona un `buen problema para principiantes`
- **Proyecto Original**: [9router by
  decolua](https://github.com/decolua/9router)

### ¿Denunciar una falla?

Al abrir una incidencia, por favor, ejecute el comando system-info y pegue el
archivo generado:

```bash
npm run system-info
```

Esto genera un `archivo de sistema-info.txt` con la versión de Node.js, la
versión de OmniRoute, detalles de sistema, herramientas CLI instaladas (si flow,
gemini, claude, códex, gravedad, dríada, etc.), estado de Docker/PM2 y paquetes
de sistema - todo lo que necesitamos para reproducir rápidamente su problema.
Pegue el archivo directamente a su problema en GitHub.

---

## Cómo funciona

```
┌─────────────┐
│  Tu herramienta CLI │  (Código del Claude, Códex, Gemini CLI, Malla abierta, Cursor, Línea del Cline)
│   herramienta     │
└──────┬──────┘
       │ http://localhost:20128/v1
       ↓
┌─────────────────────────────────────────┐
│           OmniRoute (Ruta inteligente )    │
│  • Formato de traducción (OpenAI  ⬅️  Claude) │
│  • Gestión de cuotas + Embebidos  +  Imágenes │
│  • Auto refresco de token            │
└──────┬──────────────────────────────────┘
       │
       ├─→ [Nivel 1: SUSCRIPCIÓN] Código del Claude, Códex, Gemini CLI
       │   ↓ límite de cuota agotado
       ├─→ [Nivel 2: LLAVE API] DeepSeek, Groq, xAI, Mestral, NVIDIA NIM, etc.
       │   ↓ límite presupuestario
       ├─→ [Nivel 3: Asequible ] GLM (0,6$/1M), MiniMax (0,2$/1M)
       │   ↓ límite presupuestario
       └─→ [Nivel 4: GRATIS] IFlow, Qwen, Kiro (sin límite)

Resultado: No te detenga la codificación, ahorro mínimo
```

---

## 🎯  Lo que resuelve OmniRoute - 30 puntos de dolor y casos de uso reales.

> **Todos los desarrolladores que usan herramientas de inteligencia artificial
> enfrentan estos problemas todos los días.** OmniRoute ha sido construido para
> resolverlos todos — desde sobrecoste hasta bloqueo regional, desde flujos de
> autorización rotos hasta operaciones de protocolo y observabilidad de empresa.

<details>
<summary><b>💸 1. "I pay for an expensive subscription but still get interrupted by limits"</b></summary>

Los desarrolladores pagan entre $20 y $200 al mes por el Claude Pro, el Códex
Pro o el copiloto de GitHub. Incluso pagando, hay un techo para la cuota — 5
horas de uso, límites semanales o límites de tarifa por minuto. En medio de una
sesión de codificación, el proveedor deja de responder y el desarrollador pierde
flujo y productividad.

**Cómo soluciona OmniRoute:**

- **Caída inteligente de 4 niveles** — Si la cuota de suscripción se agota,
  redirige automáticamente a Llave API → Asequible → Gratuito con cero
  intervención manual
- **Gestión de cuotas en tiempo real** — Mostrar el consumo de tokens en tiempo
  real con un recuento de reinicio (5h, diario, semanal)
- **Soporte para múltiples cuentas** — Múltiples cuentas por proveedor con
  redescansión automática — cuando una se agota, cambia a la siguiente
- **Combinaciones personalizadas** — Redes de caída personalizables con 6
  estrategias de equilibrio (primero llenado, redescansión circular, P2C,
  aleatorio, menos usado, optimizado por costo)
- **Cuotas de negocio de Codex** — Monitoreo de cuotas de negocio / Equipo de
  área de trabajo en la herramienta de dashboard

</details>

<details>
<summary><b>🔌 2. "I need to use multiple providers but each has a different API"</b></summary>

OpenAI utiliza un formato, Claude (Anthropic) utiliza otro, Gemini utiliza aún
otro. Si un desarrollador quiere probar modelos de diferentes proveedores o caer
hacia atrás entre ellos, necesitarán reconfigurarse las SDKs, cambiar los puntos
finales de las rutas, manejarse los formatos incompatible. Los proveedores
personalizados (amigoLI, NIM) tienen puntos finales de modelo no estándar

**Cómo soluciona OmniRoute:**

- **Punta final unificada** — Un único `http://localhost:20128/v1` funciona como
  proxy para todos los 67+ proveedores
- **Traducción de formato** — Automática y transparente: OpenAI  Claude 
  Gemini  API de respuesta
- **Sanurización de respuesta** — Borra los campos no estándar (`x_groq`,
  `usage_breakdown`, `service_tier`) que quebrar el SDK de OpenAI v1.83+
- **Normalización de roles** — Convierte `developer` → `system` para proveedores
  no de OpenAI; `system` → `user` para GLM/ERNIE
- ** Extracción de etiquetas de pensamiento** — Extrae `<think>` bloques del
  modelo como DeepSeek R1 en contenido de `razonamiento`</think>
- **Salida estructurada para Gemini** — `schemas de JSON` → `mimeTipo de
  respuesta`/`schema de respuesta` conversión automática
- ** `stream` por defecto se establece en `falso`** — Concuerda con la
  especificación de OpenAI, evitando el SSE inesperado en SDKs de Python, Rust y
  Go

</details>

<details>
<summary><b>🌐 3. "My AI provider blocks my region/country"</b></summary>

Los proveedores como OpenAI / Código bloquean el acceso de ciertas regiones
geográficas. Los usuarios obtienen errores como
`región_territorio_pais_desconocido` durante la OAuth y las conexiones API. Esto
es especialmente frustrante para desarrolladores de países en desarrollo.

**Cómo soluciona OmniRoute:**

- **Configuración de Proxy de Tres Niveles** — Configurable proxy en tres
  niveles: global (todo el tráfico), por proveedor (solo un proveedor) y por
  conexión/clave
- **Banderas de Proxy de Código de Colores** — Indicadores visuales: 🟢 proxy
  global, 🟡 proxy por proveedor, 🔵 proxy de conexión, mostrando siempre la IP
- **Intercambio de tokens de OAuth a través de proxy** — flujo de OAuth pasa
  también por el proxy, resolviendo `región_territorio_pais_desconocido`
- **Pruebas de conexión a través de proxy** — las pruebas de conexión utilizan
  el proxy configurado (sin más bypass directo)
- **Soporte de SOCKS5** — soporte completo de proxy SOCKS5 para la ruta de
  salida
- **Spoofing de huella de TLS** — Fingerprint de TLS como un navegador mediante
  `wreq-js` para evitar la detección de bots
- **Coincidencia automatizada de huella CLI** — Reordena los campos de
  encabezados y cuerpo para coincidir con la firma nativa de la unidad CLI
  binaria, reduciendo drásticamente el riesgo de bloqueo del account. La IP de
  la proxy se Preserve — obtiene la furtividad **h y** máscara de IP al mismo
  tiempo

</details>

<details>
<summary><b>🆓 4. "I want to use AI for coding but I have no money"</b></summary>

No todos pueden pagar $20–200/mes por suscripciones de IA. Los estudiantes, los
desarrolladores de países en desarrollo, los aficionados y los freelancers
necesitan acceso a modelos de alta calidad a cero costo.

**Cómo soluciona OmniRoute:**

- **Proveedores de Tercer Nivel Construidos por Defecto** — Soporte nativo para
  proveedores 100% gratuitos: iFlow (5 modelos ilimitados mediante OAuth:
  kimi-k2-pensamiento, qwen3-plus-coder, deepseek-r1, minimax-m2, kimi-k2), Qwen
  (4 modelos ilimitados: qwen3-plus-coder, qwen3-plus-coder-saltos,
  qwen3-next-coder, modelo de visión), Kiro (Claude + AWS Builder ID para
  gratuito), CLI de Gemini (180K tokens/mes gratuito)
- **Nubeluna en la Nube** — Nubeluna en la nube modelos Ollama en
  `api.ollama.com` con la capa de uso "luz" gratuita; use `ollamacloud/` prefijo
- **Cadenas de Combos de Solo Gratuito** — Cadenas `gc/gemini-3-salto hacia
  delante → if/kimi-k2-pensamiento → qw/qwen3-plus-coder` = $0/mes con cero
  tiempo de inactividad
- **Acceso de NVIDIA NIM de Servicio Gratuito** — ~40 RPM acceso gratuito de
  desarrollador para siempre al acceso de 70+ a modelos en build.nvidia.com (en
  transición de créditos a límites de tasa pura)
- [Estrategia Optimizada de Costos]Cost Optimized Strategy[E012E] — Estrategia
  de ruteo que automatiza la elección del proveedor más económico disponible

</details>

<details>
<summary><b>🔒 5. "I need to protect my AI gateway from unauthorized access"</b></summary>

Al exponer un gateway de AI a la red (LAN, VPS, Docker), cualquier persona con
la dirección puede consumir las claves/tarifa del desarrollador. Sin protección,
las API es vulnerables a mal uso, inyección de mensajes, abuso y manipulación.

**Cómo soluciona OmniRoute:**

- [Gestión de Claves de API]API Key Management[E015E] — Generación, rotación y
  enmascaramiento por proveedor con una página de administrador [panel de
  control/dashborad/api-manager[E087E]
- [Permisos a nivel de modelo]Model-Level Permissions[E022E] — Restringir claves
  de API a modelos específicos ([modelo abiertoai/*[E069E, patrones de
  comodín],), con el acrónimo permitir todo/Restrict.
- [Protección del punto final de API]API Endpoint Protection[E016E] — Requerir
  una clave para [/v1/models[E034E] y bloquear proveedores específicos de la
  lista
- [Guardia de Autenticación + Protección CSRF]Auth Guard + CSRF
  Protection[E013E] — Todas las rutas de consola protegidas con middleware
  [withAuth[E073E] + tokens CSRF
- [Límite de velocidad]Rate Limiter[E015E] — Limitación de velocidad por IP con
  ventanas configurables
- [Filtrado de IP]IP Filtering[E015E] — Listas blanca o negra para control de
  acceso
- [Guardia contra inyección de mensajes]Prompt Injection Guard[E023E] —
  Sanitación contra patrones de mensajes maliciosos
- [Encriptación AES-256-GCM]AES-256-GCM Encryption[E023E] — Claves criptadas en
  repositorio

</details>

<details>
<summary><b>🛑 6. "My provider went down and I lost my coding flow"</b></summary>

Los proveedores de AI pueden volverse inestables, devolver respuestas con
errores 5xx o alcanzar límites de velocidad temporales. Si un desarrollador
depende de un solo proveedor, se ve interrumpido. Sin quebradores de circuito,
intentos repetidos pueden bloquear la aplicación

**Cómo soluciona OmniRoute:**

- [Cascade a menudo por modelo con circuito breaker]Circuit Breaker
  per-model[E028E] — Auto-abrir/cerrar con umbrales configurables y cooldown
  (cerrado/abierto/media-abierta), escalado por modelo para evitar bloqueos en
  cadena cascada
- [Cosnueces exponenciales]Exponential Backoff[E021E] — Retrasos de delay de
  retries progresivos
- [Mútices de anti-estampida]Anti-Thundering Herd[E022E] — Protección de mutex +
  semáforo contra lluvias de intentos concurrentes
- [Chaines de retorno combinadas]Combo Fallback Chains[E024E] — Si el proveedor
  principal falla, cae automáticamente por la cadena con ninguna intervención
- [Cadena de circuitos a menudo]Combo Circuit Breaker[E024E] — Auto-desactiva
  proveedores fallidos dentro de una cadena de combos
- [Pantalla de monitoreo de salud]Health Dashboard[E018E] — Monitoreo de
  disponibilidad, estados del quebrador de circuito, bloqueos, estadísticas de
  caché, latencia p50/p95/p99

</details>

<details>
<summary><b>🔧 7. "Configuring each AI tool is tedious and repetitive"</b></summary>

Los desarrolladores utilizan Cursor, Claude Code, Codex CLI, OpenClaw, Gemini
CLI, Kilo Code... Cada herramienta requiere una configuración diferente (punto
final de API, clave, modelo). Reconfiguración al cambiar proveedores o modelos
es una pérdida de tiempo.

**Cómo soluciona OmniRoute:**

- **Herramientas de CLI Dashboard** — Página dedicada con una sola pantalla para
  configurar Claude Code, Codex CLI, OpenClaw, Kilo Code, Antigravity, Cline
- **Generador de Configuración de GitHub Copilot** — Genera
  `chatLanguageModels.json` para VS Code con selección de modelos en bulk
- **Asistente de inicio** — Instalación guiada de cuatro pasos para usuarios
  nuevos
- **Un endpoint, todos los modelos** — Configure `http://localhost:20128/v1` una
  sola vez, acceda a 67+ proveedores

</details>

<details>
<summary><b>🔑 8. "Managing OAuth tokens from multiple providers is hell"</b></summary>

Claude Code, Codex, Gemini CLI, Copilot — todos utilizan OAuth 2.0 con tokens
expirables. Los desarrolladores necesitan re-autenticarse constantemente,
manejan `client_secret faltante`, `redirect_uri_mismatch`, y fracasos en
servidores remotos. OAuth en una red/VPS es particularmente problemático

**Cómo soluciona OmniRoute:**

- **Actualización de tokens automatizada** — Tokens de OAuth se actualizan en
  segundo plano antes de expirar
- **OAuth 2.0 (PKCE) integrado** — Flujo automático para Claude Code, Codex,
  Gemini CLI, Copilot, Kiro, Qwen, iFlow
- **OAuth Multi-Cuenta** — Múltiples cuentas por proveedor a través de JWT/ID
  token de extracción
- **Solución de OAuth LAN/Remote** — Deteción de Dirección IP privada para
  `redirect_uri` + modo de URL manual para servidores remotos
- **Guía de OAuth detrás de Nginx** — Utiliza `window.location.origin` para
  compatibilidad con proxy de reversa
- **Guía de OAuth remota** — Guía paso a paso para credenciales de Google Cloud
  en VPS/Docker

</details>

<details>
<summary><b>📊 9. "I don't know how much I'm spending or where"</b></summary>

Los desarrolladores utilizan múltiples proveedores pagos pero no tienen una
visión unificada del gasto. Cada proveedor tiene su propio centro de
facturación, pero no hay una vista consolidada. Costos imprevistos pueden
acumularse

**Cómo soluciona OmniRoute:**

- **Panel de análisis de costos** — Seguimiento de costo por uso por modelo y
  gestión de presupuesto por proveedor
- **Límites de presupuesto por trama** — Suelo de gasto por trama que
  desencadena un fallback automático
- **Configuración de precios por modelo personalizado** — Precios
  personalizables por modelo
- **Estadísticas de uso por clave API** — Cuenta de solicitudes y último uso por
  clave
- **Panel de análisis** — Cartas de estado, gráfico de uso de modelos, tabla de
  proveedores con tasas de éxito y latencia

</details>

<details>
<summary><b>🐛 10. "I can't diagnose errors and problems in AI calls"</b></summary>

==WEBLATE_PART==\
Cuando una llamada falla, el desarrollador no sabe si fue un límite de
velocidad, token caducado, formato incorrecto o error del proveedor. Los
registros fragmentados en diferentes terminales. Sin observabilidad, el depurado
es cuestión de prueba y error.

**Cómo soluciona OmniRoute:**

- **Panel de control unificado de registros** — 4 pestañas: Registros de
  solicitud, Registros de intermediario, Registros de auditoría, Panel de
  consola
- **Visualizador de registros de consola** — Visualizador en tiempo real de
  estilo de terminal con colores codificados, auto-desplazamiento, búsqueda,
  filtro
- **Registros persistentes de intermediario de SQLite** — Registros que
  sobreviven a reinicios del servidor
- **Playa de pruebas del traductor** — 4 modos de depurado: Jardín (traducción
  de formato), Chat de pruebas (idąa y vuelta), Mesón de pruebas (lote),
  Monitoreo en vivo (en tiempo real)
- **Instrumentación de solicitud** — Retraso p50/p95/p99 + identificador de
  solicitud X-Request-Id
- **Registro basado en archivo con rotación** — Interceptor de consola captura
  todo a un registro JSON con rotación basada en tamaño
- **Informe de información del sistema** — `npm run system-info` genera
  `system-info.txt` con tu entorno completo (versión de Node, versión de
  OmniRoute, OS, herramientas CLI, estado de Docker/PM2). Adélitelo cuando
  reportes problemas para un triaje instantáneo.

</details>

<details>
<summary><b>🏗️ 11. "Deploying and maintaining the gateway is complex"</b></summary>

La instalación, configuración y mantenimiento de un proxy de inteligencia
artificial a través de diferentes entornos (local, VPS, docker, en la nube) es
laborioso. Problemas como rutas de acceso hardcoded, `EACCES` en directorios,
conflictos de puerto, y compilaciones de plataforma cruzada aumentan la
fricción.

**Cómo soluciona OmniRoute:**

- **Instalación global de npm** — `npm install -g omniroute &amp;&amp;
  omniroute` — hecho
- **Multiplataforma de Docker** — AMD64 + ARM64 nativo (Apple Silicon, AWS
  Graviton, Raspberry Pi)
- **Perfiles de Docker Compose** — `base` (sin herramientas CLI) y `cli` (con
  Claude Code, Codex, OpenClaw)
- **Application de escritorio de Electron** — Aplicación nativa para
  Windows/macOS/Linux con bandeja del sistema, arranque automático, modo sin
  conexión
- **Modo de puertos divididos** — API y Dashboard en puertos separados para
  escenarios avanzados (reverso de proxy, networking de contenedor)
- **Sincronización en la nube** — Sincronización de configuración a través de
  trabajadores de Cloudflare
- **Copias de seguridad de DB** — Copia de seguridad automática, restauración,
  exportación y importación de todas las configuraciones

</details>

<details>
<summary><b>🌍 12. "The interface is English-only and my team doesn't speak English"</b></summary>

Los equipos en países que no hablan inglés, especialmente en América Latina,
Asia y Europa, tienen dificultades con interfaces en inglés. Las barreras del
lenguaje reducen la adopción y aumentan los errores de configuración.

**Cómo soluciona OmniRoute:**

- **Panel de inicio i18n — 30 Idiomas** — Todos 500+ claves traducidas,
  incluyendo árabe, búlgaro, danés, alemán, inglés, finés, francés, hebreo,
  hindi, húngaro, indonesio, italiano, japonés, coreano, malayo, neerlandés,
  noruego, polaco, portugués (PT/BR), rumano, ruso, eslovaco, sueco, tailandés,
  ucraniano, vietnamita, chino, filipino
- **Soporte RTL** — Soporte de izquierda a derecha para árabe y hebreo
- **Multi-Lenguaje READMEs** — 30 traducciones completas de documentación
- **Selector de idioma** — Ícono de globo en la cabecera para cambiar en tiempo
  real

</details>

<details>
<summary><b>🔄 13. "I need more than chat — I need embeddings, images, audio"</b></summary>

El AI no es solo la completación de conversación. Los desarrolladores necesitan
generar imágenes, transcribir audio, crear embebes de RAG, volver a tener en
cuenta documentos, y moderar contenido. Cada API tiene un diferente punto final
y formato.

**Cómo soluciona OmniRoute:**

- **Embebes** — `/v1/embeddings` con 6 proveedores y 9+ modelos
- **Generación de imágenes** — `/v1/images/generations` con 10 proveedores y 20+
  modelos (OpenAI, xAI, Juntos, Fuego de artificio, Nebius, Hiperbólico,
  NanoBanana, Antigravedad, SD WebUI, ComfyUI)
- **Text-to-Video** — `/v1/videos/generations` — ComfyUI (AnimateDiff, SVD) y SD
  WebUI
- **Texto-a-música** — `/v1/music/generations` — ComfyUI (Audio estableabierto
  abierto, MusicGen)
- **Transcripción de audio** — `/v1/audio/transcriptions` — Whisper + Nvidia
  NIM, HuggingFace, Qwen3
- **Texto-a-habla** — `/v1/audio/speech` — ElevenLabs, Nvidia NIM, HuggingFace,
  Coqui, Tortuga, Qwen3, **Inworld**, **Cartesia**, **PlayHT**, + proveedores
  existentes
- **Moderaciones** — `/v1/moderations` — Verificaciones de seguridad de
  contenido
- **Reranking** — `/v1/rerank` — Nuevamente vuelta a tener en cuenta documentos
  para su relevancia
- **API de respuestas** — Total `/v1/responses` de soporte para Codex

</details>

<details>
<summary><b>🧪 14. "I have no way to test and compare quality across models"</b></summary>

Los desarrolladores quieren saber cuál modelo es el mejor para su caso de uso —
código, traducción, razonamiento — pero comparar manualmente es lento. No
existen herramientas de evaluación integradas.

**Cómo soluciona OmniRoute:**

- **Evaluaciones de LLM** — Prueba de conjunto dorado con 10 casos pre-cargados
  que cubren saludos, matemáticas, geografía, generación de código, cumplimiento
  JSON, traducción, markdown, refusión de seguridad
- **4 Estrategias de coincidencia** — `exacta`, `contiene`, `regex`,
  `personalizada` (función JS)
- **Parque de pruebas de Translator Playground** — Pruebas en lote con múltiples
  inputs y salidas esperadas, comparación de proveedores
- **Chat Tester** — Ronda completa al vuelta con visualización de respuesta
- **Monitoreo en vivo** — Flujo en tiempo real de todos los pedidos que fluyen a
  través del proxy

</details>

<details>
<summary><b>📈 15. "I need to scale without losing performance"</b></summary>

A medida que aumenta el volumen de solicitudes, sin caché las mismas preguntas
generan costos duplicados. Sin idempotencia, las solicitud duplicadas
desperdician recursos de procesamiento. Deben respetarse los límites de tasa por
proveedor.

**Cómo soluciona OmniRoute:**

- **Caché semántica** — Reduce costos y latencia mediante una caché
  bidireccional (firmas + semántica)
- **Idempotencia de la solicitud** — Ventana de deduplicación de 5s para
  solicitudes idénticas
- **Deteción de límites de tasa** — Seguimiento de RPM por proveedor, mínima
  brecha y máximo concurrente
- **Configuración de Límites de Tasa Editables** — Configuración por defecto
  configurable en Configuración → Resiliencia con persistencia
- **Cache de validación de llave API** — Caché de 3 niveles para rendimiento en
  producción
- **Panel de control de salud con telemetría** — Latencia p50/p95/p99,
  estadísticas de cache, disponibilidad

</details>

<details>
<summary><b>🤖 16. "I want to control model behavior globally"</b></summary>

Los desarrolladores que desean tener todas las respuestas en un idioma
específico, con un tono específico o que quieren limitar tokens de razonamiento.
Configurando esto en todas las herramientas y solicitudes es inpráctico

**Cómo soluciona OmniRoute:**

- **Inyección de Promt del Sistema** — Promt global aplicado a todas las
  solicitudes
- **Validación del presupuesto del razonamiento** — Control de asignación de
  tokens de razonamiento por solicitud (passthrough, auto, personalizado,
  adaptativo)
- **6 Estratejas de enrutamiento** — Estrategias globales que determinan cómo se
  distribuyen las solicitudes
- **Router de comodín** — Rutas dinámicas a cualquier proveedor con patrones
  `proveedor/*`
- **Deshabilitar/Activar Toggle Combinado** — Puede deshabilitar o habilitar
  combos directamente desde el panel de control
- **Tornillo de proveedor** — Conectarse/desconectarse todas las conexiones de
  un proveedor con un solo clic
- **Proveedores bloqueados** — Excluir proveedores específicos de la lista de
  `/v1/models`

</details>

<details>
<summary><b>🧰 17. "I need MCP tools as first-class product capabilities"</b></summary>

Muchos gateways de inteligencia artificial exponen MCP solo como un detalle de
implementación oculto. Los equipos necesitan un capa de operaciones visible y
gestionable.

**Cómo soluciona OmniRoute:**

- Menú de navegación en la consola (MCP) y protocolo de fin de punto
- Página de gestión exclusiva de MCP con proceso, herramientas, alcance y
  auditoría
- Iniciación rápida integrada para omniroute --mcp[] y inicio de cliente

</details>

<details>
<summary><b>🧠 18. "I need A2A orchestration with sync + stream task paths"</b></summary>

Necesidad de flujos de trabajo de agentes con respuestas directas y ejecuciones
streamadas de larga duración con control de vida

**Cómo soluciona OmniRoute:**

- Punto final JSON-RPC de A2A ([POST /a2a[]]) con mensajes/enviar[] y
  mensajes/flujo[]
- Streaming en tiempo real con propagación del estado terminal
- API de ciclo de vida para tareas con tareas/[get[]] y tareas/cancelar[]

</details>

<details>
<summary><b>🛰️ 19. "I need real MCP process health, not guessed status"</b></summary>

Los equipos operativos necesitan saber si MCP está realmente activo, no solo si
una API es accesible

**Cómo soluciona OmniRoute:**

- Archivo de latido de tiempo de ejecución con PID, horarios de tiempo,
  transporte, número de herramientas y modo de alcance
- API de estado de MCP combinando latido + actividad reciente
- Tarjetas de estado en la interfaz de usuario para proceso/uptime/actualización
  de latido

</details>

<details>
<summary><b>📋 20. "I need auditable MCP tool execution"</b></summary>

Cuando las herramientas mutan la configuración o dispara acciones de
operaciones, los equipos necesitan trazabilidad forense

**Cómo soluciona OmniRoute:**

- Control de auditoría por medio de un registro de SQLite de llamadas de
  herramientas de MCP
- Filtro por herramienta, éxito/fallo, clave de API y navegación
- Tabla de auditoría de la consola + finales de estadísticas para automatización

</details>

<details>
<summary><b>🔐 21. "I need scoped MCP permissions per integration"</b></summary>

Los diferentes clientes deben tener acceso de privilegios mínimos a categorías
de herramientas.

**Cómo soluciona OmniRoute:**

- 9 escopos granulares MCP para acceso controlado a herramientas
- Cumplimiento y visibilidad del alcance en la interfaz de usuario de gestión de
  MCP
- Postura de seguridad predeterminada para herramientas de operación

</details>

<details>
<summary><b>⚙️ 22. "I need operational controls without redeploying"</b></summary>

Las equipos necesitan cambios de ejecución rápidos durante incidentes o eventos
de costo.

**Cómo soluciona OmniRoute:**

- Activación de la combinación de interruptoresdirectamente desde la consola MCP
- Aplicar perfiles de resistencia desde paquetes de políticas definidas
  previamente
- Restablecer el estado del interruptor de circuito desde el mismo panel de
  operaciones

</details>

<details>
<summary><b>🔄 23. "I need live A2A task lifecycle visibility and cancellation"</b></summary>

Sin visibilidad de ciclo de vida, las incidentes de tarea se vuelven difíciles
de triar.

**Cómo soluciona OmniRoute:**

- Listado y filtrado de tareas por estado/habilidad con paginación
- Herramienta de bajada en profundidad del metadato de tarea, eventos y
  artefactos
- Fin de la tarea con confirmación con fin de tarea y fondo

</details>

<details>
<summary><b>🌊 24. "I need active stream metrics for A2A load"</b></summary>

Los flujos de trabajo en línea requieren visión operativa sobre la concurrencia
y conexiones vivas.

**Cómo soluciona OmniRoute:**

- Contadores de flujo activo integrados en el panel de estado A2A
- Último timestamp de tarea y conteos por estado
- Tarjetas del tablero de A2A para monitoreo de operaciones en tiempo real

</details>

<details>
<summary><b>🪪 25. "I need standard agent discovery for clients"</b></summary>

Los clientes y orquestadores externos necesitan metadatos de máquina leídos para
la incorporación.

**Cómo soluciona OmniRoute:**

- Tarjeta de Agente expuesta en `/.well-known/agent.json`
- Capacidades y habilidades mostradas en la interfaz de administración
- El API de estado A2A incluye metadatos de descubrimiento para automatización

</details>

<details>
<summary><b>🧭 26. "I need protocol discoverability in the product UX"</b></summary>

Si los usuarios no pueden descubrir superficies de protocolo, la calidad de
adopción y soporte disminuye.

**Cómo soluciona OmniRoute:**

- Página consolidada de endpoints **Endpoints** con pestañas para Proxy, MCP,
  A2A y Endpoints de API
- Alternadores de estado de servicio en línea (en línea/offline) para MCP y A2A
  en el mismo lugar
- Enlaces desde vista general a tablas de gestión dedicadas

</details>

<details>
<summary><b>🧪 27. "I need end-to-end protocol validation with real clients"</b></summary>

Los pruebas de simulación no son suficientes para validar la compatibilidad de
protocolo antes de la liberación.

**Cómo soluciona OmniRoute:**

- Sistema de prueba E2E que inicia la aplicación y utiliza el cliente de
  trasporte SDK de MCP real
- Pruebas del cliente A2A para descubrimiento, enviar, transmisor, obtener y
  cancelar
- Comprueba las afirmaciones cruzadamente contra las APIs de auditoría de MCP y
  las tareas de A2A

</details>

<details>
<summary><b>📡 28. "I need unified observability across all interfaces"</b></summary>

La división de observabilidad por protocolo crea puntos ciegos y errores de MTTR
más largos.

**Cómo soluciona OmniRoute:**

- Conjuntos de tableros sanos registradores/analíticos en un producto
- Trazabilidad + auditoría + telemetría de solicitudes a través de los capas de
  OpenAI, MCP y A2A
- Las API operativas para estado y automatización

</details>

<details>
<summary><b>💼 29. "I need one runtime for proxy + tools + agent orchestration"</b></summary>

Correr muchos servicios separados aumenta el coste operativo y los modos de
fallo.

**Cómo soluciona OmniRoute:**

- Proveedor de proxy compatible con OpenAI, servidor MCP y servidor A2A en una
  sola pila
- Autenticación compartida, resistencia, almacenamiento de datos e informes de
  observación
- Modelo de políticas coherente en todas las superficies de interacción

</details>

<details>
<summary><b>🚀 30. "I need to ship agentic workflows without glue-code sprawl"</b></summary>

Los equipos pierden velocidad cuando configuran múltiples servicios y scripts
ad-hoc.

**Cómo soluciona OmniRoute:**

- Estrategia de endpoint unificado para clientes y agentes
- Interfaces de usuario de gestión de protocolos integradas y rutas de
  validación de humo
- Fundamentos listos para producción (seguridad, registro de actividad,
  resistencia, copia de seguridad)

</details>

### Ejemplos de Playbooks (Uso de casos integrados)

**Playbook A: Maximizar suscripción con pago + respaldo barato**

```txt
Combo: "maximize-claude"
  1. cc/claude-opus-4-6
  2. glm/glm-4.7
  3. if/kimi-k2-thinking

Costo mensual: $20 + gastar poco en respaldo
Resultado: calidad más alta, prácticamente cero interrupción
```

**Playbook B: Marco de codificación de costo cero**

```txt
Combo: "free-forever"
  1. gc/gemini-3-flash
  2. if/kimi-k2-thinking
  3. qw/qwen3-coder-plus

Costo mensual: $0
Resultado: flujo de codificación estable y gratuito
```

**Playbook C: Cadena de respaldo 24/7 siempre encendida**

```txt
Combo: "always-on"
  1. cc/claude-opus-4-6
  2. cx/gpt-5.2-codex
  3. glm/glm-4.7
  4. minimax/MiniMax-M2.1
  5. if/kimi-k2-thinking

Resultado: profundidad de respaldo profunda para cargas de trabajo críticas y de plazo
```

**Playbook D: Operaciones de agente con MCP + A2A**

```txt
1) Inicie el transporte MCP (`omniroute --mcp`) para operaciones impulsadas por herramientas
2) Ejecutar tareas A2A vía `message/send` y `message/stream`
3) Observar vía /dashboard/endpoint (pantallas MCP y A2A)
4) Activar servicios vía controles de estado inline
```

---

## 🆓 Ingreso Gratuito — Sin Costo de Configuración

> Configure codificación AI en minutos por $0 al mes**. Conecte estas cuentas
> gratuitas y utilice el combo integrado **Free Stack**.

| Paso | acción                                                        | Proveedores Desbloqueados                                         |
| ---- | ------------------------------------------------------------- | ----------------------------------------------------------------- |
| 1    | Conecta **Kiro** (ID de acceso OAuth del Constructor de AWS)  | Sonieta de Claude 4.5, Haiku 4.5 — **ilimitados**                 |
| 2    | Conecta **iFlow** (OAuth de Google)                           | pensamiento-k2, qwen3-coder-plus, deepseek-r1... — **ilimitados** |
| 3    | Conecta **Qwen** (Código de dispositivo)                      | qwen3-coder-plus, qwen3-coder-flash... — **ilimitados**           |
| 4    | Conecta **CLI de Gemini** (OAuth de Google)                   | gemini-3-flash, gemini-2.5-pro — **180K/mes gratis**              |
| 5    | `/dashboard/combos` → **Pila gratuita (0 USD)** de plantillas | Redondea automáticamente todos los proveedores gratuitos          |

**Punte cualquier IDE/CLI a:** `http://localhost:20128/v1` · Llave de API:
`cualquier-string` · Listo.

> **Cobertura adicional opcional (también gratuita):** Llave API de Groq (30 RPM
> gratis), NVIDIA NIM (40 RPM gratis, 70+ modelos), cerebros (1M tok/día), Llave
> de API de LongCat (50M tokens/día!).

## Inicio rápido

### 1. Instalar y ejecutar

```bash
npm install -g omniroute
omniroute
```

> **pnpm usuarios:** Ejecute `pnpm approve-builds -g` después de la instalación
> para habilitar scripts de compilación nativos requeridos por `better-sqlite3`
> y `@swc/core`:
> 
> ```bash
> pnpm install -g omniroute
> pnpm approve-builds -g   # Selecciona todos los paquetes → aprobar
> omniroute
> ```

La consola de dashboard se abre en `http://localhost:20128` y la ruta base de la
API es `http://localhost:20128/v1`.

| Comando                   | Descripción                                                          |
| ------------------------- | -------------------------------------------------------------------- |
| `omniroute`               | Inicia servidor (`PUERTO=20128`, API y dashboard en el mismo puerto) |
| `omniroute --puerto 3000` | Establecer puertocanonical/API a 3000                                |
| `omniroute --mcp`         | Inicia servidor MCP (transporte estándar)                            |
| `omniroute --no-abierto`  | No se abre automáticamente la navegador                              |
| `omniroute --ayuda`       | Mostrar ayuda                                                        |

Opción de modo de puerto dividido:

```bash
PUERTO=20128 DASHBOARD_PORT=20129 omniroute
# API:       http://localhost:20128/v1
# Dashboard: http://localhost:20129
```

### 1) Conecta proveedores y crea tu clave de API

1. Abre el panel de control → `Proveedores` y conecta al menos un proveedor
   (OAuth o clave de API).
2. Abre el panel de control → `Puntos de conexión` y crea una clave de API.
3. ( OPCIONAL ) Abre el panel de control → `Combinaciones` y establece tu cadena
   de fallback.

### 2) Pinta tu herramienta de programación hacia OmniRoute

```txt
Dirección base: http://localhost:20128/v1
Clave de API:  [copia de la página de puntos de conexión]
Modelo:    if/kimi-k2-pensamiento (o cualquier prefijo de proveedor/modelo)
```

Funciona con Claude Code, Codex CLI, Gemini CLI, Cursor, Cline, OpenClaw,
OpenCode y SDK compatibles con OpenAI.

### 3) Habilita y valida los protocolos (v2.0)

**MCP (para operaciones impulsadas por herramientas):**

```bash
omniroute --mcp
```

Luego conecta tu cliente MCP sobre `stdio` y prueba herramientas como:

- `omniroute_get_salud`
- `omniroute_list_combos`

**A2A (para flujos de agentes a agentes):**

```bash
curl http://localhost:20128/.well-known/agency.json
```

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'content-type: application/json' \
  -d '{"jsonrpc":"2.0","id":"quickstart","method":"message/send","params":{"skill":"gestión_de_cuotas","messages":[{"role":"usuario","content":"Dame un resumen de cuota corto."}]}}'
```

### 4) Valida todo de punta a punta (recomendado)

```bash
npm run test:protocolos:e2e
```

Esta suite valida flujos de cliente MCP y A2A reales contra una aplicación en
ejecución.

### O alternativa: corre desde la fuente.

```bash
cp .env.example .env
npm install
PORT=20128 DASHBOARD_PORT=20129 NEXT_PUBLIC_BASE_URL=http://localhost:20129 npm run dev
```

---

## 🐳 Docker

OmniRoute is available as a public Docker image on [Docker
Hub](https://hub.docker.com/r/diegosouzapw/omniroute).

**Quick run:**

```bash
docker run -d \
  --name omniroute \
  --restart unless-stopped \
  -p 20128:20128 \
  -v omniroute-data:/app/data \
  diegosouzapw/omniroute:latest
```

**With environment file:**

```bash
# Copy and edit .env first
cp .env.example .env

docker run -d \
  --name omniroute \
  --restart unless-stopped \
  --env-file .env \
  -p 20128:20128 \
  -v omniroute-data:/app/data \
  diegosouzapw/omniroute:latest
```

**Using Docker Compose:**

```bash
# Base profile (no CLI tools)
docker compose --profile base up -d

# CLI profile (Claude Code, Codex, OpenClaw built-in)
docker compose --profile cli up -d
```

| Imagen                   | Tag      | Tamaño | Descripción           |
| ------------------------ | -------- | ------ | --------------------- |
| `diegosouzapw/omniroute` | `latest` | ~250MB | Latest stable release |
| `diegosouzapw/omniroute` | `1.0.3`  | ~250MB | Current version       |

---

## 🖥️ Desktop App — Offline & Always-On

> 🆕 **NUEVO!** OmniRoute ahora está disponible como una **aplicación de
> escritorio nativa** para Windows, macOS y Linux.

Ejecuta OmniRoute como una aplicación de escritorio independiente — sin
terminal, sin navegador, sin conexión a Internet necesaria para modelos locales.
La aplicación basada en Electron incluye:

- 🖥️ **Ventana Nativa** — Ventana de aplicación dedicada con integración de área
  de notificación del sistema
- 🔄 **Inicio Automático** — Inicia OmniRoute a la hora de inicio del sistema
- 🔔 **Notificaciones Nativas** — Obtiene notificaciones sobre agotamiento de
  cuota o problemas con proveedor
- ⚡ **Instalación con un Solo Click** — NSIS (Windows), DMG (macOS), AppImage
  (Linux)
- 🌐 **Modo de Oficina** — Funciona completamente de forma offline con servidor
  embutido

### Inicio rápido

```bash
#  Modo de desarrollo
npm run electron:dev

#  Edición para tu plataforma
npm run electron:build         # Plataforma actual
npm run electron:build:win     # Windows (.exe)
npm run electron:build:mac     # macOS (.dmg) — x64 &amp; arm64
npm run electron:build:linux   # Linux (.AppImage)
```

### Barra de Tareas

Al minimizar, OmniRoute vive en tu barra de tareas con acciones rápidas:

- Abrir panel
- Cambiar puerto del servidor
- Salir de la aplicación

📖 Documentación completa: [`electron/README.md`](electron/README.md)

---

## Tarifa en Vistaz de Ojos

| Nivel              | Proveedor                                   | Costo                           | Reiniciar Cuota   | Mejor para                                    |
| ------------------ | ------------------------------------------- | ------------------------------- | ----------------- | --------------------------------------------- |
| **💳 SUSCRIPCIÓN**  | Claude Código (Pro)                         | $20/mes                         | 5h + semanal      | Ya suscrito                                   |
|                    | Codex (Plus/Pro)                            | $20-200/mes                     | 5h + semanal      | Navegadores de OpenAI                         |
|                    | CLI de Gemini                               | **GRAFITIS**                    | 180K/mes + 1K/día | ¡Todo el mundo!                               |
|                    | Copiloto de GitHub                          | $10-19/mes                      | Mensual           | Usuarios de GitHub                            |
| **🔑 CLAVE DE API** | NVIDIA NIM                                  | **GRAFITIS** (dev para siempre) | ~40 RPM           | 70+ modelos abiertos                          |
|                    | Cerebras                                    | **GRATIS** (1M tok/día)         | 60K TPM / 30 RPM  | Lo más rápido del mundo                       |
|                    | Groq                                        | **GRATIS** (30 RPM)             | 14.4K RPD         | Llama/Gemma ultrarrápido                      |
|                    | DeepSeek V3.2                               | $0.27/$1.10 por 1M              | Ninguno           | Mejor precio/razón de calidad                 |
|                    | xAI Grok-4 Rapido                           | **$0.20/$0.50 por 1M** 🆕        | Ninguno           | Rápido + llamada a herramientas, bajísimo     |
|                    | xAI Grok-4 (estándar)                       | $0.20/$1.50 por 1M 🆕            | Ninguno           | Flamante de razón de xAI                      |
|                    | Mistral                                     | Gratuito + pago                 | Tarifa limitada   | IA europeo                                    |
|                    | OpenRouter                                  | Según el uso                    | Ninguno           | Más de 100 modelos en conjunto                |
| ** 💰 BARATO **     | GLM-5 (a través de Z.AI) 🆕                  | $0.5/1M                         | Cada 10AM, diario | 128K salidas, bandera de la última generación |
|                    | GLM-4.7                                     | $0.6/1M                         | Cada 10AM, diario | Backup-presupuesto                            |
|                    | MiniMax M2.5 🆕                              | $0.3/1M de entrada              | 5-horas en rodaje | Tareas de razonamiento + agente               |
|                    | MiniMax M2.1                                | $0,2/1M                         | 5-horas en rodaje | Opción más barata                             |
|                    | Kimi K2.5 (Moonshot API) 🆕                  | Según el uso                    | Ninguno           | Acceso directo a la Moonshot API              |
|                    | Kimi K2                                     | $9/mes fijo                     | 10M tokens/mes    | Costo predecible                              |
| **🆓 GRATIS**       | iFlow                                       | **$0**                          | Sin límite        | 5 modelos ilimitados                          |
|                    | Qwen                                        | **$0**                          | Sin límite        | 4 modelos ilimitados                          |
|                    | Kiro                                        | **$0**                          | Sin límite        | Claude Sonnet/Haiku (AWS Builder)             |
|                    | LongCat Flash-Lite 🆕                        | **$0** (50M tok/día 🔥)          | 1 RPS             | La cuota más grande gratuita en la Tierra     |
|                    | Polinización AI                             | **$0** (no clave necesaria)     | 1 req/15s         | GPT-5, Claude, DeepSeek, Llama 4              |
|                    | Cloudflare Workers AI                       | **$0** (10K neuronas/día)       | ~150 resp/día     | 50+ modelos, red de borde global              |
|                    | Escala de trabajo inteligente de Cloudflare | **$0** (1M tokens totales)      | Tarifa limitada   | UE / RGPD, Qwen3 235 GB, Llama 70 GB          |

> **Nuevo modelo agregado (mar 2026):** familia rápida Grok-4 Flash a
> $0,20/$0,50/ M (marcado en 1143 ms — 30% más rápido que Gemini 2.5 Flash),
> GLM-5 a través de Z.AI con 128K de salida, MiniMax M2.5 razonamiento, DeepSeek
> V3.2 precio actualizado, Kimi K2.5 a través de API directa Moonshot.

**💡 Combo pila gratuita $0 — La configuración completa gratuita:**

```
# 🆓 Pila gratuita final 2026 
Eligió Kiro (kr/)             → Hada Sonnet/Claude UNLIMITADO
elegir iFlow (if/)            → kimi-k2-pensamiento, qwen3-coder-plus, deepseek-r1 SELECCIONADO
 eligió LongCat Lite (lc/)     → LongCat-Flash-Lite — 50 GB/día 🔥
eligió Pollinations (pol/)    → GPT-5, Claude, DeepSeek, Llama 4 — sin clave necesaria
eligió Qwen (qw/)             → qwen3-coder-plus, qwen3-coder-flash, qwen3-coder- Siguiente SELECCIONADO
eligió Gemini (gemini/)       → Gemini 2.5 Flash — 1.500 req/día clave API gratuita
eligió Cloudflare AI (cf/)    → Llama 70 GB, Gemma 3, Mistral — 10K Neuronas/día
eligió Escala (scw/)           → Qwen3 235B, Llama 70 GB — 1M tokens gratis (UE)
eligió Groq (groq/)           → Llama / Gemma ultra-rápida — 14.4K req/día
 Eligió NVIDIA NIM (nvidia/)   → 70+ modelos abiertos — 40 RPM por siempre
eligió Cerebras (cerebras/)   → Llama / Qwen el mundo rápido — 1M tok/día
```

**Precio cero. Nunca se detiene codificando.** Configura esto como una
combinación de combo de OmniRoute y todos los redireccionamientos de backup
suceden automáticamente — no hay manual intercambio nunca.

---

---

## 🆓 Modelos gratis — Lo que obtienes realmente en efecto

> Todos los modelos a continuación son **100% gratis con cero tarjeta de crédito
> necesaria**. OmniRoute redirige automáticamente entre ellos cuando se agota
> una cuota — combina todos los modelos para un combo de $0 inquebrantable.

### 🔵 MODELOS DE CLAUDE (a través de Kiro — Builder ID de AWS)

| modelo              | Prefijo | limit         | Límite de tarifa                              |
| ------------------- | ------- | ------------- | --------------------------------------------- |
| `claude-sonnet-4.5` | `kr/`   | **Ilimitado** | No se ha reportado ninguna restricción diaria |
| `claude-haiku-4.5`  | `kr/`   | **Ilimitado** | No se ha reportado ninguna restricción diaria |
| `claude-opus-4.6`   | `kr/`   | **Ilimitado** | Ópera más reciente a través de Kiro           |

### 🟢 MÓDULOS IFLOW (OAuth gratuito — Sin tarjeta de crédito)

| modelo                    | Prefijo | limit         | Límite de tarifa                       |
| ------------------------- | ------- | ------------- | -------------------------------------- |
| `kimi-k2-thinking`        | `if/`   | **Ilimitado** | No se ha reportado ninguna restricción |
| `qwen3-coder-plus`        | `if/`   | **Ilimitado** | No se ha reportado ninguna restricción |
| `busqueda-en-deepseek-r1` | `if/`   | **Ilimitado** | No se ha reportado ninguna restricción |
| `minimagrupación-2.1`     | `if/`   | **Ilimitado** | No se ha reportado ninguna restricción |
| `kimi-k2`                 | `if/`   | **Ilimitado** | No se ha reportado ninguna restricción |

### 🟡 MODELOS QWEN (Código de autenticación del dispositivo)

| modelo                          | Prefijo | limit         | Límite de tarifa                       |
| ------------------------------- | ------- | ------------- | -------------------------------------- |
| `qwen3-coder-plus`              | `qw/`   | **Ilimitado** | No se ha reportado ninguna restricción |
| `qwen3-codificadores-plasma`    | `qw/`   | **Ilimitado** | No se ha reportado ninguna restricción |
| `qwen3-codificadores-siguiente` | `qw/`   | **Ilimitado** | No se ha reportado ninguna restricción |
| `modelo-vision`                 | `qw/`   | **Ilimitado** | Multimodal (imágenes)                  |

### 🟣 GEMINI CLI (Google OAuth)

| modelo                               | Prefijo | limit                        | Límite de tarifa |
| ------------------------------------ | ------- | ---------------------------- | ---------------- |
| `gemini-3-previsualización de flash` | `gc/`   | **180K tok/mes** + 1K/día    | Reseteo mensual  |
| `gemini-2.5-pro`                     | `gc/`   | 180K/mes (bloque compartido) | Alta calidad     |

### ⚫ NVIDIA NIM (Contraseña de API gratuita — build.nvidia.com)

| Nivel                  | Límite diario       | Límite de tarifa | Notas                                                          |
| ---------------------- | ------------------- | ---------------- | -------------------------------------------------------------- |
| Gratis (Desarrollador) | Sin límite de token | **~40 RPM**      | 70+ modelos;  transición a límites de tasa puros a junio, 2025 |

Modelos de texto gratuitos populares: `moonshotai/kimi-k2.5` (Kimi K2.5),
`z-ai/glm4.7` (GLM 4.7), `deepseek-ai/deepseek-v3.2` (DeepSeek V3.2),
`nvidia/llama-3.3-70b-instruct`, `deepseek/deepseek-r1`

### ⚪ CEREBRAS (Contraseña de API gratuita — inference.cerebras.ai)

| Nivel  | Límite diario        | Límite de tarifa | Notas                                                              |
| ------ | -------------------- | ---------------- | ------------------------------------------------------------------ |
| Gratis | **1M tokens/al día** | 60K TPM / 30 RPM | La inferencia del LLM más rápida del mundo; se resetea diariamente |

Disponible de forma gratuita: `llama-3.3-70b`, `llama-3.1-8b`,
`deepseek-r1-distill-llama-70b`

### 🔴 GROQ (Clave de API gratuita — console.groq.com)

| Nivel  | Límite diario  | Límite de tarifa  | Notas                                                   |
| ------ | -------------- | ----------------- | ------------------------------------------------------- |
| Gratis | **14.4KM RPD** | 30 RPM por modelo | Sin tarjeta de crédito; 429 en el límite, no se cobrará |

Disponible de forma gratuita: `llama-3.3-70b-versatile`, `gemma2-9b-it`,
`mixtral-8x7b`, `whisper-large-v3`

### 🔴 LONGCAT AI (Clave de API gratuita — longcat.chat) 🆕

| modelo                        | Prefijo | Cupo diario gratuito | Notas                               |
| ----------------------------- | ------- | -------------------- | ----------------------------------- |
| `LongCat-Flash-Lite`          | `lc/`   | **50M tokens** 💥     | Cuota gratuita más grande en efecto |
| `LongCat-Flash-Chat`          | `lc/`   | 500K tokens          | Conversación multivuelta            |
| `LongCat-Flash-Thinking`      | `lc/`   | 500K tokens          | Razonamiento / CoT                  |
| `LongCat-Flash-Thinking-2601` | `lc/`   | 500K tokens          | Versión de enero 2026               |
| `LongCat-Flash-Omni-2603`     | `lc/`   | 500K tokens          | Multimodal                          |

> 100% de cobertura mientras en beta pública. Regístrate en
> [longcat.chat](https://longcat.chat) con correo electrónico o teléfono. Se
> resetea diariamente a las 00:00 UTC.

### 🟢 POLINIZACIONES AI (No se requiere una clave API) 🆕

| modelo     | Prefijo | Límite de tarifa | Proveedor detrás   |
| ---------- | ------- | ---------------- | ------------------ |
| `openai`   | `pol/`  | 1 req/15s        | GPT-5              |
| `claude`   | `pol/`  | 1 req/15s        | Anthropic Claude   |
| `gemini`   | `pol/`  | 1 req/15s        | Google Gemini      |
| `deepseek` | `pol/`  | 1 req/15s        | DeepSeek V3        |
| `llama`    | `pol/`  | 1 req/15s        | Meta Llama 4 Scout |
| `mistral`  | `pol/`  | 1 req/15s        | Mistral AI         |

> ✨ **Sin fricción cero:** No se necesita matrícula, ni API. Agregar el
> proveedor de Pollinations con un campo de clave vacío y funciona de inmediato.

### 🟠 CLOUDFLARE WORKERS AI (Clave API gratuita — cloudflare.com) 🆕

| Nivel  | Neuronas diarias | Equivalente de uso                                      | Notas                   |
| ------ | ---------------- | ------------------------------------------------------- | ----------------------- |
| Gratis | **10,000**       | ~150 LLM por respuesta / 500s de audio / 15K de embebes | Orea edgía, 50+ modelos |

Modelos populares gratuitos: `@cf/meta/llama-3.3-70b-instruct`,
`@cf/google/gemma-3-12b-it`, `@cf/openai/whisper-large-v3-turbo` (audio
gratis!), `@cf/qwen/qwen2.5-coder-15b-instruct`

> Requiere token de API + ID de cuenta desde
> [dash.cloudflare.com](https://dash.cloudflare.com). Almacena el ID de cuenta
> en configuración del proveedor.

### 🟣 SCALEWAY AI (1M Tokens Gratuitos — scaleway.com) 🆕

| Nivel  | Cuota gratuita | Ubicación    | Notas                                                   |
| ------ | -------------- | ------------ | ------------------------------------------------------- |
| Gratis | **1M tokens**  | 🇫🇷 París, EU | No se requiere tarjeta de crédito dentro de los límites |

Disponible gratis: `qwen3-235b-a22b-instruct-2507` (Qwen3 235B!),
`llama-3.1-70b-instruct`, `mistral-small-3.2-24b-instruct-2506`,
`deepseek-v3-0324`

> Cumple con la GDPR/UE. Obtén la clave de API en
> [console.scaleway.com](https://console.scaleway.com).

> **💡 La Pila Libre Total (11 Proveedores, $0 Para Siempre):**
> 
> ```
> Kiro (kr/)             → Claude Sonnet/Haiku ILIMITADO
> iFlow (if/)            → kimi-k2-pensamiento, qwen3-código-plus, deepseek-r1 ILIMITADO
> LongCat Lite (lc/)     → LongCat-Flash-Lite — 50M tokens/día 🔥
> Pollinations (pol/)    → GPT-5, Claude, DeepSeek, Llama 4 — no key necesario
> Qwen (qw/)             → qwen3-modelos de ceder ilimitados
> Gemini (gemini/)       → Gemini 2.5 Flash — 1.500 req/día gratuito
> Cloudflare AI (cf/)    → 50+ modelos — 10K Neuronas/día
> Scaleway (scw/)        → Qwen3 235B, Llama 70B — 1M tokens gratuitos (EU)
> Groq (groq/)           → Llama/Gemma — 14,4K req/día ultra-rápido
> NVIDIA NIM (nvidia/)   → 70+ modelos abiertos — 40 RPM en perpetuidad
> Cerebras (cerebras/)   → Llama/Qwen el más rápido del mundo — 1M tok/día
> ```

## 🎙️ Mezcla de Transcripción Gratuita

> Transcribir cualquier audio/video por **$0** — Deepgram lidera con $200
> gratis, AssemblyAI $50 de respaldo, Groq Whisper como respaldo de emergencia
> ilimitado.

| Proveedor        | Créditos Gratuitos         | Mejor Modelo                                | Límite de tarifa                            |
| ---------------- | -------------------------- | ------------------------------------------- | ------------------------------------------- |
| 🟢 **Deepgram**   | **$200 gratis** (registro) | `nova-3` — mejor exactitud, 30+ idiomas     | Sin limitación en RPM de créditos gratuitos |
| 🔵 **AssemblyAI** | **$50 gratis** (registro)  | `universal-3-pro` — capítulos, opinión, PII | Sin limitación en RPM de créditos gratuitos |
| 🔴 **Groq**       | **Gratis para siempre**    | `whisper-large-v3` — OpenAI Whisper         | 30 RPM (limitado por tasa)                  |

**Combo sugerida en `/dashboard/combos`:**

```
Nombre: transcripción-gratuita
Estrategia: Prioridad
Nodos:
  [1] deepgram/nova-3          → utiliza $200 gratis primero
  [2] assemblyai/universal-3-pro → respaldo cuando los créditos de Deepgram agoten
  [3] groq/whisper-large-v3    → gratis para siempre, respaldo de emergencia
```

Entonces en `/Dashboard/Media` → **Transcripción** pestaña: subir cualquier
archivo de audio o video → seleccionar su punto final de conexión → obtener la
transcripción en formatos compatibles.

## 💡 Características Clave

OmniRoute v2.0 se construye como una plataforma operativa, no solo como un proxy
de relay.

### 🆕 Nuevo — Mejoras Inspiradas en ClawRouter (Mar 2026)

| Característica                                    | ¿Qué hace?                                                                                                                                |
| ------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- |
| ⚡ **Familia Grok-4 Rápida**                       | Modelos AI a $0.20/$0.50/M — medidos 1143ms (30% más rápido que Gemini 2.5 Flash)                                                         |
| 🧠 **GLM-5 a través de Z.AI**                      | Contexto de salida de 128K, $0.5/1M — la bandera más nueva de la familia GLM                                                              |
| 🔮 **MiniMax M2.5**                                | Tareas de razonamiento + agente a $0.30/1M — actualización significativa desde M2.1                                                       |
| 🎯 **Bandera de llamada a herramienta por modelo** | Llamada de herramienta por modelo por `toolCalling: verdadero/falso` en el registro — AutoCombo ignora modelos no capaces de herramientas |
| 🌍 **Deteción de intención multilingüe**           | Palabras clave en PT/ZH/ES/AR en la puntuación de AutoCombo — selección de modelo mejorada para contenido no inglés                       |
| 📊 **Fallas impulsadas por benchmarks**            | Latencia real p95 de solicitudes en vivo alimenta la puntuación de combo — AutoCombo aprende de datos reales                              |
| 🔁 **Deduplicación de solicitudes**                | Ventana de deduplicación basada en hash de contenido — seguro para agentes múltiples, previene cobros duplicados                          |
| 🔌 **Estrategia de Router Pluggable**              | Extensible `Estrategia de Router` interface — agregue lógica de routing personalizada como plugins                                        |

### 🚀 Anterior a v2.0.9+ — Playground, CLI Dedos y ACP

| Característica                                     | ¿Qué hace?                                                                                                                                                                                                                                                                                                                 |
| -------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🎮 **Modelo Playground**                            | Página de dashboard para probar cualquier modelo directamente — seleccionadores de proveedor/modelo/punto final, Editor Monaco, streaming, aborto, puntaje                                                                                                                                                                 |
| 🔏 **CLI Coincide con Huella Física**               | Reordenamiento de cabeceras/cuerpos por proveedor para coincidir con firmas nativas de CLI — activar por proveedor en Configuración > Seguridad. **Su IP de proxy se preserva**                                                                                                                                            |
| 🤝 **Soporte de ACP (Protocolo de Agente Cliente)** | Descubrimiento de agente CLI (Codex, Claude, Goose, Gemini CLI, OpenClaw + 9 más), lanzador de proceso, `/api/acp/agentes` punto final                                                                                                                                                                                     |
| 🤖 **Panel de Agentes de ACP**                      | Depuración › Página de Agentes — cuadricula de 14 agentes con estado de instalación, versión, formulario de agente personalizado para cualquier herramienta CLI. **usuarios de OpenCode** obtienen un botón "Descargar opencode.json" que auto-genera una configuración lista para usar con todos los modelos disponibles. |
| 🔧 **Ruta de Modelos `apiFormat` Personalizada**    | Modelos personalizados con `apiFormat: "respuestas"` ahora se dirigen correctamente al traductor de respuestas API                                                                                                                                                                                                         |
| 🏢 **Codex Workspace de Aislamiento**               | Trabajos de Codex multiples por correo electrónico — OAuth separa conexiones correctamente por ID de trabajo                                                                                                                                                                                                               |
| 🔄 **Actualización Electrónica Automática**         | La aplicación de escritorio verifica actualizaciones + automantente en arranque                                                                                                                                                                                                                                            |

### 🤖 Operaciones del Agente y el Protocolo (v2.0)

| Característica                                                   | ¿Qué hace?                                                                                                       |
| ---------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| 🔧 **Servidor MCP (16 herramientas)**                             | IDE/tools del agente a través de 3 transportes: stdio, SSE (`/api/mcp/sse`), HTTP Streamable (`/api/mcp/stream`) |
| 🤝 **Servidor A2A (JSON-RPC + SSE)**                              | Ejecución de tareas entre agentes con flujos sincrónicos y en flujo continuo                                     |
| 🧭 **Página de puntos de conexión consolidados**                  | Página de administración con tarjetas para Proxies de Puntos de conexión, MCP, A2A y Puntos de conexión de API   |
| 🎚️ **Alternadores de habilitación/deshabilitación de servicios** | Interruptores ON/OFF para MCP y A2A con persistencia de ajustes (predeterminado: OFF)                            |
| 🛰️ **Latido del tiempo de ejecución de MCP**                     | Estado real del proceso (pid, tiempo de ejecución, edad de latido, transporte, modo de alcance)                  |
| 📋 **Rastro de auditoría MCP**                                    | Registros de auditoría filtrables con atribución de éxito/falla y clave                                          |
| 🔐 **Cumplimiento del alcance de MCP**                            | 9 permisos de alcance granulares para acceso controlado a herramientas                                           |
| 📡 **Gestión de la vida de los tareas A2A**                       | Lista y filtra tareas, inspecciona eventos/artefactos, cancela tareas en ejecución                               |
| 📋 **Descubrimiento de tarjetas de agente**                       | `/.well-known/agent.json` para descubrimiento automático del cliente                                             |
| 💡 **Protocolo E2E Prueba de Harness**                            | Real MCP SDK + A2A client flows en `test:protocols:e2e`                                                          |
| ⚙️ **Controles Operativos**                                      | Combos de interruptores, aplicar perfiles de resistencia, resetear interruptores desde una superficie de control |

### 💡 Ruteo y Inteligencia

| Característica                               | ¿Qué hace?                                                                                             |
| -------------------------------------------- | ------------------------------------------------------------------------------------------------------ |
| 🎯 **fallback Inteligente 4 Echelones**       | Ruta automática: Suscripción → Clave API → Barato → Gratuito                                           |
| 📊 **Monitoreo en tiempo real de cuotas**     | Conteo de tokens en vivo + cuenta regresiva de reinicio por proveedor                                  |
| 🔄 **Traducción de formato**                  | OpenAI ↔ Claude ↔ Gemini ↔ Conversiones seguras con schema                                             |
| 👥 **Soporte para cuentas múltiples**         | Múltiples cuentas por proveedor con selección inteligente                                              |
| 🔄 **Renovación automática de tokens**        | Los tokens OAuth se renuevan automáticamente con reintentos                                            |
| 🎨 **Combos personalizados**                  | 6 estrategias de equilibrio + control de cadena de respaldo                                            |
| 🌐 **Routeador wildcard**                     | `proveedor/*` ruteo dinámico                                                                           |
| 🧠 **Presupuesto de Control del Pensamiento** | Paso a través, automático, personalizado y límites de razón adaptativos                                |
| 🔀 **Aliados de Modelo**                      | Alios de modelado integrados + de migración y seguridad personalizados                                 |
| ⚡ **Decaimiento de Fondo**                   | En rutas de tareas de fondo de baja prioridad a modelos más baratos                                    |
| 🧪 **Smart Routing con Consciencia de Tarea** | Selecciona automáticamente modelo por tipo de contenido (codificación/análisis de visión/sumarización) |
| 💬 **Inyección de Promedio del Sistema**      | Controles de comportamiento global aplicados consistentemente                                          |
| 📄 **Compatibilidad de la API de Respuestas** | Completos `/v1/responses` para Codex y flujo de trabajo agente avanzado                                |

### 🎵 API Multi-Modal

| Característica                | ¿Qué hace?                                                                                                                                                                                |
| ----------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🖼️ **Generación de Imágenes** | `/v1/images/generations` con backends cloud y locales                                                                                                                                     |
| 📐 **Embebidos**               | `/v1/embeddings` para flujos de trabajo de búsqueda y de RAG                                                                                                                              |
| 🎤 **Transcripción de Audio**  | `/v1/audio/transcripciones` — 7 prestadores (Deepgram Nova 3, AssemblyAI, Groq Whisper, HuggingFace, ElevenLabs, OpenAI, Azure), detección automática de idioma, soporte para MP4/MP3/WAV |
| 🔊 **Texto a Voz**             | `/v1/audio/texto-a-voz` — 10 prestadores (ElevenLabs, OpenAI, Deepgram, Cartesia, PlayHT, HuggingFace, Nvidia NIM, Inworld, Coqui, Tortoise) con mensajes de error correctos              |
| 🎬 **Generación de Vídeos**    | `/v1/videos/generaciones` (ComfyUI + SD WebUI workflows)                                                                                                                                  |
| 🎵 **Generación de Música**    | `/v1/music/generaciones` (ComfyUI workflows)                                                                                                                                              |
| 🛡️ **Moderaciones**           | `/v1/moderaciones` verificaciones de seguridad                                                                                                                                            |
| 🔀 **Reranking**               | `/v1/rerank` para puntuación de relevancia                                                                                                                                                |
| 🔍 **Búsqueda en la Web** 🆕    | `/v1/busqueda` — 5 prestadores (Serper, Brave, Perplexity, Exa, Tavily), 6,500+ gratuitos/mes, falla automática, caché                                                                    |

### 🛡️ Resiliencia, Seguridad & Gobernanza

| Característica                                            | ¿Qué hace?                                                                                                |
| --------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- |
| 🔌 **Resortes de Circuito**                                | Toma de viaje/recover por modelo con controles de umbral                                                  |
| 🎯 **Modelos Conscientes de Puntos de Fin**                | 🛡️ [X3X] Protección contra el Estallido de Trueno [X25X]                                                  |
| Mútuo + protecciones de semáforo en eventos de retry/rate | Reducción de costes/diferenciales de latencia con dos capas de caché                                      |
| 🧠 ** Caché semántica + Signatura **                       | Protección contra duplicados con ventana de tiempo                                                        |
| ⚡ ** Idoneidad de Solicitud **                            | Protectora ventana de tiempo de duplicados                                                                |
| 🔒 ** Spoofing de Huella de TLS **                         | Fingerprint de TLS nativo del navegador — ** reduce riesgos de detección de bots y flagging de cuentas ** |
| 🔏 **CLI Coincide con Huella Física**                      | Coincide con firmas de solicitud nativas CLI — ** reduce el riesgo de banido preservando IP de proxy **   |
| 🌐 ** Filtros de IP **                                     | Control de listas de permitidos/denegados para despliegues expuestos                                      |
| 📊 ** Limites de Tasa Editables **                         | Limites globales/nivel de proveedor configurables con persistencia                                        |
| 🔑 ** Administración de Claves API + Escopes **            | Emisión de claves seguras/giro y controles de proveedores y modelos                                       |
| 🛡️ ** /modelos protegidos**                               | Autenticación opcional con ocultación de proveedores para catálogo de modelos                             |

### 📊 Observabilidad y Análisis

| Característica                                | ¿Qué hace?                                                                |
| --------------------------------------------- | ------------------------------------------------------------------------- |
| 📝 **Solicitud + Registros de Proxy**          | Logos completos de solicitud/response y registro de proxy                 |
| 📋 **Panel de Mosaicos de Registro Unificado** | Vistas de solicitud, proxy, auditoría y consola en una página             |
| 🔍 **Telemetría de Solicitudes**               | Latencia de p50/p95/p99 y rastreo de solicitudes                          |
| 🏥 **Panel de Mía [Dashboard de Salud]**       | Diseño de tiempo, estados de breaker, bloqueos, estadísticas de caché     |
| 💰 **Seguimiento de Costos**                   | Control de presupuestos y visibilidad de precios por modelo               |
| 📈 **Visualizaciones de Análisis**             | Insights del uso de modelos/proveedores y vistas de tendencia             |
| 🧪 ** Marco de Evaluación**                    | Pruebas del conjunto dorado con estrategias de coincidencia configurables |

### ☁️ Inicio y Plataforma

| Característica                                    | ¿Qué hace?                                                                                                             |
| ------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- |
| 🌐 **Despliega en Cualquier Lugar**                | Localhost, VPS, Docker, Entornos de la nube                                                                            |
| 💾 Rendimiento de **Cloud Sync**                   | Sincronización de configuración mediante worker de la nube                                                             |
| 🔄 **Backup/Restore**                              | Flujo de exportación e importación y recuperación en caso de desastre                                                  |
| 🧙 **Mesa de ayuda para la configuración inicial** | Asistencia guiada para la primera ejecución                                                                            |
| 🔧 ** Ventana de herramientas CLI**                | Configuración con un solo clic para herramientas de programación populares                                             |
| 🎮 **Modelo Playground**                           | Puedes probar cualquier proveedor/m Modelo/punto final desde la ventana de la consola                                  |
| 🔏 **Deshacer el pulgar digital de la CLI**        | Coincidencia del pulgar digital por proveedor en Configuración > Seguridad                                             |
| 🌐 **i18n (30 idiomas)**                           | Soporte completo del idioma en la barra de herramientas + documentación con capacidad de texto derechos a la izquierda |
| 🧹 ** Vaciar toda la lista de modelos**            | Borrar automáticamente la lista de modelos en los detalles del proveedor                                               |
| 📋 **Plantillas de problemas**                     | Plantillas de GitHub estándar para bugs y características                                                              |
| 📂 **Directorio de datos personalizado**           | `DIRECTORIO_DE_DATOS` para superposición de ubicación de almacenamiento                                                |

### Avance de Funcionalidad

#### Fallo hacia atrás inteligente con control de costos prácticos

```txt
Combo: "mi-pila-de-código"
  1. cc/claude-opus-4-6
  2. nvidia/llama-3.3-70b
  3. glm/glm-4.7
  4. if/kimi-k2-pensando
```

Cuando la cuota, la tasa o la salud fallan, OmniRoute se mueve automáticamente a
la siguiente candidata sin cambiar manualmente.

#### Administrar protocolos visibles y operables

- MCP + A2A son descubridos en la interfaz y en los documentos (no ocultos)
- Las APIs de estado de protocolo exponen datos de operación en vivo
  (`/api/mcp/*`, `/api/a2a/*`)
- Los tableros de control incluyen acciones para operaciones de día 2
  (combinaciones de interruptores, reinicios de circuito, cancelación de tareas)

#### Flujo de trabajo de traductor + validación

La zona de traductor incluye:

- ** Play Ground**: solicitar verificaciones de transformación
- ** Chat Tester**: viaje completo de solicitud y respuesta
- ** Prueba de Borda**: varios casos en una sola ejecución
- ** Monitor en tiempo real**: vista de tráfico en tiempo real

Además, la validación de protocolos con clientes reales a través de ` npm run
test:protocolos:e2e`.

> 📖 **[README del Servidor MCP](open-sse/mcp-server/README.md)** — Referencia de
> herramienta, configuraciones de IDE y ejemplos de clientes
> 
> 📖 **[README del Servidor A2A](src/lib/a2a/README.md)** — Habilidades, métodos
> JSON-RPC, transmisión y ciclo de vida de tareas

## Evaluaciones (Evals)

OmniRoute incluye un marco de evaluación integrado para probar la calidad de las
respuestas de LLM contra un conjunto de oro. Acceda a él a través de ** Análisis
→ Evaluación** en el tablero de control.

### Conjunto de oro integrado

El conjunto de oro "OmniRoute" predeterminado contiene casos de prueba para:

- Saludos, matemáticas, geografía, generación de código
- Cumplimiento del formato JSON, traducción, generación de markdown
- Rechazo a seguridad (contenido dañino), conteo, lógica booleana

### Estrategias de evaluación

| Estrategia      | Descripción                                                                   | Ejemplo                                |
| --------------- | ----------------------------------------------------------------------------- | -------------------------------------- |
| `exacto`        | La salida debe coincidir exactamente                                          | `"4"`                                  |
| `contiene`      | La salida debe contener una subcadena (in sensible a mayúsculas y minúsculas) | `"París"`                              |
| `regex`         | La salida debe coincidir con un patrón de expresión regular                   | `"1.*2.*3"`                            |
| `personalizado` | La función de JavaScript personalizada devuelve Verdadero/Falso               | `(output) =&gt; output.length &gt; 10` |

---

## Guía de configuración 📖

### Configuración de protocolo (MCP + A2A)

<details>
<summary><b>🧩 MCP Setup (Model Context Protocol)</b></summary>

Inicia el transporte de MCP en modo de interfaz de la consola:

```bash
omniroute --mcp
```

Flujo de validación recomendado:

1. Conecta tu cliente de MCP a través de la interfaz de la consola.
2. Ejecuta `omniroute_get_health`.
3. Ejecuta `omniroute_list_combos`.
4. Abre `/dashboard/mcp` para confirmar el latido, la actividad y la auditoría.

APIs útiles para la automación:

- `GET /api/mcp/status`
- `GET /api/mcp/tools`
- `GET /api/mcp/audit`
- `GET /api/mcp/audit/stats`

</details>

<details>
<summary><b>🤝 A2A Setup (Agent2Agent)</b></summary>

Descubre al agente:

```bash
curl http://localhost:20128/.well-known/agency.json
```

Envía una tarea:

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'content-type: application/json' \
  -d '{"jsonrpc":"2.0","id":"setup-a2a","method":"message/send","params":{"skill":"quota-management","messages":[{"role":"user","content":"Summarize quota status."}]}}'
```

Administra la vida ciclica:

- `GET /api/a2a/estado`
- `GET /api/a2a/tareas`
- `GET /api/a2a/tareas/:id`
- `POST /api/a2a/tareas/:id/cancelar`

Interfaz de usuario de funcionamiento:

- `/dashboard/a2a` para la observabilidad de tareas/estado/emisores y acciones
  de humo

</details>

<details>
<summary><b>🧪 End-to-end protocol validation</b></summary>

Verifica ambas protocolos con clientes reales:

```bash
npm run test:protocolos:e2e
```

Esto verifica:

- Cliente SDK MCP conecta/lista/llamada
- Descubrimiento A2A/enviar/emisores/obtener/cancelar
- Comprueba los datos en los auditorías de MCP y las API de gestión de tareas
  A2A

</details>

<details>
<summary><b>💳 Subscription Providers</b></summary>

### Claude Código (Pro/Max)

```bash
Dashboard → Proveedores → Conectar Claude Código
→ Inicio de sesión de OAuth → Actualización automática de token
→ Seguimiento del límite + semanal 5 horas

Modelos:
  cc/claude-opus-4-6
  cc/claude-sonnet-4-5-20250929
  cc/claude-haiku-4-5-20251001
```

**Consejo pro:** Utiliza Opus para tareas complejas, Sonnet para velocidad.
OmniRoute sigue el seguimiento del límite por modelo

### Código de Codex de OpenAI (Plus/Pro)

```bash
Dashboard → Proveedores → Conectar Codex
→ Inicio de sesión de OAuth (puerto 1455)
→ Reseteo semanal + de 5 horas

Modelos:
  cx/gpt-5.2-codex
  cx/gpt-5.1-codex-max
```

#### Administración de políticas de cuenta de Código de Codex (5h + Semanal)

Ahora cada cuenta de Codex tiene palancas de política en `Dashboard -&gt;
Proveedores`:

- `5 horas` (ACTIVADO/OF): aplica la política del umbral de 5 horas.\
  ==WEBLATE_PART==
- `Semanal` (ON/OFF): establece la política de umbral de ventana semanal.
- Comportamiento de umbral: cuando una ventana habilitada alcanza >=90% de uso,
  la cuenta se omite.
- Comportamiento de rotación: OmniRoute redirige a la próxima cuenta de Codex
  elegible automáticamente.
- Comportamiento de reinicio: cuando pasa el tiempo de reinicio del proveedor
  `resetAt`, la cuenta se hace elegible nuevamente automáticamente.

Escenarios:

- `5h ON` + `Semanal ON`: la cuenta se omite cuando alcanza cualquiera de los
  umbrales.
- `5h OFF` + `Semanal ON`: solo el uso semanal puede bloquear la cuenta.
- `5h ON` + `Semanal OFF`: solo el uso de 5 horas puede bloquear la cuenta.
- `resetAt` ha pasado: la cuenta reingresa la rotación automáticamente (no es
  necesaria una reactivación manual).

### Gemini CLI (FREE 180K/month!)

```bash
Dashboard → Proveedores → Conectar Gemini CLI
→ Google OAuth
→ 180K completaciones/mes + 1K/día

Modelos:
  gc/gemini-3-flash-preview
  gc/gemini-2.5-pro
```

**Mejor Valor:** ¡Tamaño de tarifa gratuita gigante! Utiliza esto antes de las
capas de tarifa pagadas.

### Copiloto de GitHub

```bash
Dashboard → Proveedores → Conectar GitHub
→ OAuth vía GitHub
→ Reseteo mensual (1.ª del mes)

Modelos:
  gh/gpt-5
  gh/claude-4.5-sonnet
  gh/gemini-3-pro
```

</details>

<details>
<summary><b>🔑 API Key Providers</b></summary>

### NVIDIA NIM (Acceso gratuito del desarrollador — 70+ modelos)

1. Regístrate: [build.nvidia.com](https://build.nvidia.com)
2. Obtén tu API Key (1000 créditos de inferencia incluidos)
3. Dashboard → Agregar Proveedor → NVIDIA NIM:
   - Clave de API: `nvapi-tu-clave`

**Modelos:** `nvidia/llama-3.3-70b-instruct`, `nvidia/mistral-7b-instruct` y 50+
más

**Consejo:** API compatible con OpenAI — se integra perfectamente con la
traducción de formato de OmniRoute!

### DeepSeek

1. Regístrate: [platform.deepseek.com](https://platform.deepseek.com)
2. Obtén una clave API
3. Panel de control → Agregar proveedor → DeepSeek

**Modelos:** `deepseek/deepseek-chat`, `deepseek/deepseek-coder`

### Groq (Disponible con el Nivel Gratuito)

1. Regístrate: [console.groq.com](https://console.groq.com)
2. Obtén una clave API (incluido el nivel gratuito)
3. Panel de control → Agregar proveedor → Groq

**Modelos:** `groq/llama-3.3-70b`, `groq/mixtral-8x7b`

**Consejo:** Inferencia ultra-rápida — lo mejor para codificación en tiempo
real!

### OpenRouter (100+ Modelos)

1. Regístrate: [openrouter.ai](https://openrouter.ai)
2. Obtén una clave API
3. Panel de control → Agregar proveedor → OpenRouter

**Modelos:** Accede a 100+ modelos de todos los proveedores principales mediante
una sola clave de API.

</details>

<details>
<summary><b>💰 Cheap Providers (Backup)</b></summary>

### GLM-4.7 (Reiniciado diariamente, $0,6/1M)

1. Regístrate: [Zhipu AI](https://open.bigmodel.cn/)
2. Obtén la clave API del Plan de Código
3. Panel de cuadro → Agregar clave API:
   - Proveedor: `glm`
   - Clave API: `tu-clave`

**Use:** `glm/glm-4.7`

**Consejo pro:** El plan de codificación ofrece 3 veces la cuota a 1/7 del
costo! Reinciar diariamente a las 10:00 a.m.

### MiniMax M2.1 (reinicia 5h, $0,20/1M)

1. Regístrate: [MiniMax](https://www.minimax.io/)
2. Obtén una clave API
3. Panel de cuadro → Agregar clave API

**Use:** `minimax/MiniMax-M2.1`

**Consejo pro:** Opción más barata para contexto largo (1 millón de tokens)!

### Kimi K2 ( $9/mes fijo)

1. Suscribirse: [Moonshot AI](https://platform.moonshot.ai/)
2. Obtén una clave API
3. Panel de cuadro → Agregar clave API

**Use:** `kimi/kimi-último`

**Consejo pro:** $9/mes fijo por 10 millones de tokens = $0,90/1 millón de
tokens de costo efectivo!

</details>

<details>
<summary><b>🆓 FREE Providers (Emergency Backup)</b></summary>

### iFlow (5 modelos gratuitos mediante OAuth)

```bash
Panel de cuadro → Conectar iFlow
→ Iniciar sesión con OAuth de iFlow
→ Uso ilimitado

 Modelos:
  if/kimi-k2-pensando
  if/qwen3-código-plus
  if/glm-4.7
  if/minimax-m2
  if/deepseek-r1
```

### Qwen (4 modelos gratuitos mediante Código de un dispositivo)

```bash
Dashboard → Conectar a Qwen
→ Autorización de código de dispositivo
→ Uso ilimitado

Modelos:
  qw/qwen3-coder-plus
  qw/qwen3-coder-flash
```

### Kiro (Claude GRATIS)

```bash
Dashboard → Conectar a Kiro
→ ID de Constructor de AWS o Google/GitHub
→ Uso ilimitado

Modelos:
  kr/claude-sonnet-4.5
  kr/claude-haiku-4.5
```

</details>

<details>
<summary><b>🎨 Create Combos</b></summary>

### Ejemplo 1: Maximar la Suscripción → Reserva Asequible

```
Dashboard → Opciones → Crear Nuevo

Nombre: codificación premium
Modelos:
  1. cc/claude-opus-4-6 (Principal de la suscripción)
  2. glm/glm-4.7 (Reserva económica, $0,6/1 millón)
  3. minimax/MiniMax-M2.1 (Renvío más económico, $0,20/1 millón)

Usar en CLI: codificación premium
```

### Ejemplo 2: Solo Gratuito (Cero Costo)

```
Nombre: Free-Only
Modelos:
  1. gc/gemini-3-flash-preview (180K mensuales gratis)
  2. if/kimi-k2-thinking (ilimitado)
  3. qw/qwen3-coder-plus (ilimitado)

Costo: $0 para siempre!
```

</details>

<details>
<summary><b>🔧 CLI Integration</b></summary>

### Cursor IDE

```
Configuración → Modelos → Avanzado:
  URL base de OpenAI API: http://localhost:20128/v1
  Clave de OpenAI API: [desde la Consola de OmniRoute]
  Modelo: cc/claude-opus-4-6
```

### Código Claude

Use la página de ** Herramientas CLI ** en la Consola para una configuración de
un solo clic, o edite `~/.claude/settings.json` manualmente.

### CLI de Codex

```bash
export OPENAI_BASE_URL="http://localhost:20128"
export OPENAI_API_KEY="tu-llave-omniroute-api"

codex "tu prompt"
```

### OpenClaw

**Opción 1 — Consola (recomendada):**

```
Consola → Herramientas de CLI → OpenClaw → Seleccionar Modelo → Aplicar
```

**Opción 2 — Manual:** Editar `~/.openclaw/openclaw.json`:

```json
{
  "modelos": {
    "proveedores": {
      "omniroute": {
        "baseUrl": "http://127.0.0.1:20128/v1",
        "apiKey": "sk_omniroute",
        "api": "openai-completions"
      }
    }
  }
}
```

> **Nota:** OpenClaw solo funciona con OmniRoute local. Usa `127.0.0.1` en lugar
> de `localhost` para evitar problemas de resolución de direcciones IPv6.

### Línea de Comandos / Continuar / RooCode

```
Configuración de API:
  Proveedor: Compatible con OpenAI
  Dirección Base: http://localhost:20128/v1
  API Key: [de la consola OmniRoute]
  Modelo: if/kimi-k2-pienso
```

### Desarrollador Aperto

**Paso 1:** Agregar OmniRoute como proveedor personalizado:

```bash
desarrolladoresaperto
/conectar
# Seleccionar "Otros" → Ingrese ID: "omniroute" → Ingrese su clave API OmniRoute
```

**Paso 2:** Crear/Editar `desarrolladoresaperto.json` en la raíz de su proyecto:

```json
{
  "$schema": "https://desarrolladoresaperto.ai/config.json",
  "proveedor": {
    "omniroute": {
      "npm": "@ai-sdk/openai-compatible",
      "nombre": "OmniRoute",
      "opciones": {
        "baseURL": "http://localhost:20128/v1"
      },
      "modelos": {
        "cc/claude-sonnet-4-20250514": { "nombre": "Claude Sonnet 4" },
        "gg/gemini-2.5-pro": { "nombre": "Gemini 2.5 Pro" },
        "if/kimi-k2-pienso": { "nombre": "Kimi K2 (Gratis)" }
      }
    }
  }
}
```

**Paso 3:** Seleccionar el modelo en Desarrollador Aperto:

```bash
/modelos
# Seleccionar cualquier modelo de OmniRoute de la lista
```

> **Consejo:** Agregar cualquier modelo disponible en su punto de conexión
> OmniRoute `/v1/modelos` a la sección `modelos`. Utilice el formato
> `proveedor/modelo-identificador` desde su consola OmniRoute.

</details>

---

## Solución de problemas

<details>
<summary><b>Click to expand troubleshooting guide</b></summary>

**"El modelo de lenguaje no proporcionó mensajes."**

- Quota de proveedor agotada → Verificar rastreador de cuota de la consola
- Solución: Utilizar fallback en combinación o cambiar a una cinta más baja

**Limitación de velocidad**

- Cuota de suscripción agotada → Regresar a GLM/MiniMax
- Agregar combo: `cc/claude-opus-4-6 → glm/glm-4.7 → if/kimi-k2-pienso`

**Token OAuth expiró**

- Automaticamente reconectado por OmniRoute
- Si persisten los problemas: Consola → Proveedor → Reiniciar conexión

**Costos altos**

- Verifique los estadísticas de uso en Menú Principal → Costos
- Cambie el modelo principal a GLM/MiniMax
- Use la versión gratuita (Gemini CLI, iFlow) para tareas no críticas

**Dashboard/API ports are wrong**

- `PORT` es el puerto base canonical (y el puerto de la API por defecto)
- `API_PORT` solo sobrelarga el escuchador de la API compatible con OpenAI
- `DASHBOARD_PORT` solo sobrelarga el escuchador de la interfaz de
  usuario/NEXT.js
- Establezca `NEXT_PUBLIC_BASE_URL` a su URL de la interfaz de usuario/public
  (para llamadas de autenticación OAuth)

**Cloud sync errors**

- Verifique `BASE_URL` que apunta a su instancia en ejecución
- Verifique `CLOUD_URL` que apunte a su endpoint en la nube esperado
- Mantenga `NEXT_PUBLIC_*` alineados con los valores del lado del servidor

**First login not working**

- Revisar `INITIAL_PASSWORD` en `.env`
- Si no está definido, la contraseña por defecto es `123456`

**No request logs**

- Establezca `ENABLE_REQUEST_LOGS=true` en `.env`

**Connection test shows "Invalid" for OpenAI-compatible providers**

- Muchos proveedores no exponen un `/models` endpoint
- OmniRoute v1.0.6+ incluye una validación de fallback a través de
  completaciones de chat
- Requerir URL base incluir el sufijo `/v1`

### Acceder mediante OAuth a un Servidor Remoto

<a name="oauth-on-a-remote-server"></a> <a name="oauth-em-servidor-remoto"></a>

> **⚠️ Importante para usuarios que ejecutan OmniRoute en un VPS, Docker, o
> cualquier servidor remoto**

#### ¿Por qué falla la autenticación de Antigravity / Gemini CLI OAuth en servidores remotos?

Los proveedores **Antigravity** y **Gemini CLI** utilizan **Google OAuth 2.0**.
Google requiere que el `ícono de redirección` en el flujo de OAuth coincida
exactamente con uno de los URIs registrados previamente en la consola de Google
Cloud.

Los credenciales de OAuth incluidas en OmniRoute están registradas **solo para
`localhost`**. Cuando accede a OmniRoute en un servidor remoto (por ejemplo,
`https://omniroute.myserver.com`), Google rechaza la autenticación con el error:

```
Error 400: el valor del parámetro `redirect_uri` no coincide con ninguno de los registros autorizados
```

#### Solución: Configura tus propias credenciales de OAuth

Necesitas crear un **identificador de cliente OAuth 2.0** en la consola de
Google Cloud con el URI de tu servidor.

#### Paso a paso

**1. Inicia sesión en la consola de Google Cloud**

Ir a:
[https://console.cloud.google.com/apis/credentials](https://console.cloud.google.com/apis/credentials)

**2. Crea un nuevo identificador de cliente OAuth 2.0**

- Haz clic en **"Crear credenciales"->** → **"Identificador de cliente OAuth"
- Tipo de aplicación: **"Aplicación web"**
- Nombre: cualquier cosa que desees (por ejemplo, `OmniRoute remoto`)

**3. Agregar URI de redirección autorizados**

En el campo [X15X]"URI de redirección autorizados"**, agrega:

```
https://tu-servidor.com/callback
```

> Sustituye `tu-servidor.com` con el dominio de tu servidor o su dirección IP
> (incluye el puerto si es necesario, por ejemplo,
> `http://45.33.32.156:20128/callback`).

**4. Guardar y copiar las credenciales**

Después de crear, Google mostrará el **ID de cliente** y el **secret de
cliente**.

**5. Establecer variables de entorno**

En tu [.env]` (o variables de entorno del contenedor Docker):

```bash
# Para Antigravity:
ANTIGRAVITY_OAUTH_CLIENT_ID=your-client-id.apps.googleusercontent.com
ANTIGRAVITY_OAUTH_CLIENT_SECRET=GOCSPX-your-secret

# Para Gemini CLI:
GEMINI_OAUTH_CLIENT_ID=your-client-id.apps.googleusercontent.com
GEMINI_OAUTH_CLIENT_SECRET=GOCSPX-your-secret
GEMINI_CLI_OAUTH_CLIENT_SECRET=GOCSPX-your-secret
```

**6. Reiniciar OmniRoute**

```bash
# npm:
npm run dev

# Docker:
docker restart omniroute
```

**7. Intenta conectarte de nuevo**

Panel de control → Proveedores → Antigravity (o Gemini CLI) → OAuth

Google ahora se redirigirá correctamente a `https://your-server.com/callback`.

---

#### Solutión temporal (sin credenciales personalizadas)

Si no deseas establecer tus propias credenciales en este momento, todavía puedes
usar el **flujo de URL manual**:

1. OmniRoute abre la URL de autorización de Google
2. Después de autorizar, Google intenta redirigirse a `localhost` (que falla en
   el servidor remoto)
3. **Copiar la URL completa** del cuadro de direcciones de tu barra de
   direcciones del navegador (incluso si no se carga la página)
4. Pega esa URL en el campo mostrado en el modal de conexión de OmniRoute
5. Haz clic en **"Conectar"**

> Esto funciona porque el código de autorización en la URL es válido
> independientemente de si se cargó la página de redirección.

---

<details>
<summary><b>🇧🇷 Versão em Português</b></summary>

#### Por qué el OAuth de Antigravity / Gemini CLI falla en servidores remotos?

Los proveedores **Antigravity** y **Gemini CLI** usan **OAuth 2.0 de Google**
para autenticación. El Google exige que la `redirect_uri` usada en el flujo
OAuth sea **exactamente** una de las URIs registradas previamente en el Google
Cloud Console del aplicativo.

As credenciales OAuth embutidas en OmniRoute están registradas **só para
`localhost`**. Cuando usted accede a OmniRoute en un servidor remoto (por
ejemplo: `https://omniroute.meuservidor.com`), Google rechaza la autenticación
con:

```
Error 400: el valor del parámetro `redirect_uri` no coincide con ninguno de los registros autorizados
```

#### Solución: Configure sus propias credenciales OAuth

Usted necesita crear un **cliente de OAuth 2.0** en Google Cloud Console con la
URI de su servidor.

#### Paso a paso

**1. Acceda a Google Cloud Console**

Abra:
[https://console.cloud.google.com/apis/credentials](https://console.cloud.google.com/apis/credentials)

**2. Cree un nuevo cliente de OAuth 2.0**

- Haga clic en **"+ Crear credenciales"** → **"Cliente de OAuth"**
- Tipo de aplicación: **"Aplicación web"**
- Nombre: elija cualquier nombre (por ejemplo: `OmniRoute Remoto`)

**3. Agregue las URL de redireccionamiento autorizadas**

En el campo **"URLs de redireccionamiento autorizadas"**, agregue:

```
https://su-servidor.com/callback
```

> Sustituya `su-servidor.com` por el dominio o IP de su servidor (incluya la
> puerta si es necesario, por ejemplo: `http://45.33.32.156:20128/callback`).

**4. Guarde y copie las credenciales**

Después de crear, Google mostrará el **ID de cliente** y el **Secret de
cliente**.

**5. Establezca las variables de entorno**

En su `.env` (o en las variables de entorno de Docker):

```bash
# Para Antigravity:
ANTIGRAVITY_OAUTH_CLIENT_ID=su-client-id.apps.googleusercontent.com
ANTIGRAVITY_OAUTH_CLIENT_SECRET=GOCSPX-su-secreto

# Para Gemini CLI:
GEMINI_OAUTH_CLIENT_ID=su-client-id.apps.googleusercontent.com
GEMINI_OAUTH_CLIENT_SECRET=GOCSPX-su-secreto
GEMINI_CLI_OAUTH_CLIENT_SECRET=GOCSPX-su-secreto
```

**6. Reinicie o OmniRoute**

```bash
# Se usando npm:
npm run dev

# Se usando Docker:
docker restart omniroute
```

**7. Tente conectar novamente**

Dashboard → Providers → Antigravity (ou Gemini CLI) → OAuth

Agora o Google redirecionará corretamente para
`https://seu-servidor.com/callback` e a autenticação funcionará.

---

#### Workaround temporário (sem configurar credenciais próprias)

Se não quiser criar credenciais próprias agora, ainda é possível usar o fluxo
**manual de URL**:

1. O OmniRoute abrirá a URL de autorização do Google
2. Após você autorizar, o Google tentará redirecionar para `localhost` (que
   falha no servidor remoto)
3. **Copie a URL completa** da barra de endereço do seu browser (mesmo que a
   página não carregue)
4. Cole essa URL no campo que aparece no modal de conexão do OmniRoute
5. Clique em **"Connect"**

> Este workaround funciona porque o código de autorização na URL é válido
> independente do redirect ter carregado ou não.

</details>

---

</details>

## 🛠️ Tech Stack

<details>
<summary><b>Click to expand tech stack details</b></summary>

- **Runtime**: Node.js 18–22 LTS (⚠️ Node.js 24+ is **not supported** —
  `better-sqlite3` native binaries are incompatible)
- **Language**: TypeScript 5.9 — **100% TypeScript** across `src/` and
  `open-sse/` (zero `any` in core modules since v2.0)
- **Framework**: Next.js 16 + React 19 + Tailwind CSS 4
- **Database**: LowDB (JSON) + SQLite (domain state + proxy logs + MCP audit +
  routing decisions)
- **Schemas**: Zod (MCP tool I/O validation, API contracts)
- **Protocols**: MCP (stdio/HTTP) + A2A v0.3 (JSON-RPC 2.0 + SSE)
- **Transmisión**: Server-Sent Events (SSE)
- **Autenticación**: OAuth 2.0 (PKCE) + JWT + Claves API + Autorización de
  ámbito de MCP
- **Pruebas**: Ejecutor de pruebas de Node.js + Vitest (900+ pruebas, incluidas
  unitarias, de integración y E2E)
- **CI/CD**: GitHub Actions (auto publicar npm + Docker Hub en la realización)
- **Sitio web**: [omniroute.online](https://omniroute.online)
- **Paquete**:
  [npmjs.com/package/omniroute](https://www.npmjs.com/package/omniroute)
- **Docker**:
  [hub.docker.com/r/diegosouzapw/omniroute](https://hub.docker.com/r/diegosouzapw/omniroute)
- **Resiliencia**: Medidor de circuito, alivio exponencial, anti-lluvia de
  tormenta, falsificación de TLS, auto-combo auto-curación

</details>

---

## Documentación

| Documentar                                     | Descripción                                                                |
| ---------------------------------------------- | -------------------------------------------------------------------------- |
| [Guía del usuario](docs/USER_GUIDE.md)         | Proveedores, combos, integración de la línea de comandos, despliegue       |
| [Referencia de la API](docs/API_REFERENCE.md)  | Todos los puntos de conexión con ejemplos                                  |
| [MCP Server](open-sse/mcp-server/README.md)    | 16 Herramientas de MCP, configs de IDE, clientes de Python/TS/Go           |
| [A2A Server](src/lib/a2a/README.md)            | Protocolo 2.0 JSON-RPC, habilidades, transmisión, administración de tareas |
| [Motor de auto-combo](docs/auto-combo.md)      | 6-puntuaje de scoring, conjuntos de modo, curación automática              |
| [Troubleshooting](docs/TROUBLESHOOTING.md)     | Problemas y soluciones comunes                                             |
| [Architecture](docs/ARCHITECTURE.md)           | Arquitectura y aspectos internos del sistema                               |
| [Contributing](CONTRIBUTING.md)                | Instalación de desarrollo y pautas                                         |
| [OpenAPI Spec](docs/openapi.yaml)              | Especificación de OpenAPI 3.0                                              |
| [Security Policy](SECURITY.md)                 | Informes de vulnerabilidad y prácticas de seguridad                        |
| [VM Deployment](docs/VM_DEPLOYMENT_GUIDE.md)   | Guía completa: configuración de VM + nginx + Cloudflare                    |
| [Features Gallery](docs/FEATURES.md)           | Tour de dashboard visual con pantallazos                                   |
| [Release Checklist](docs/RELEASE_CHECKLIST.md) | Paso a paso de validación previa al lanzamiento                            |

---

## 🗺️ Mapa de ruta

OmniRoute tiene **210+ características planificadas** en varias etapas de
desarrollo. A continuación, se muestran las áreas clave:

| Categoría                          | Funciones Planeadas | Destacados                                                                                                         |
| ---------------------------------- | ------------------- | ------------------------------------------------------------------------------------------------------------------ |
| 🧠 **Rutas & Inteligencia**         | 25+                 | Rruteo de menor latencia, ruteo basado en etiquetas, prefiltro de cuotas, selección de cuenta P2C                  |
| 🔒 **Seguridad & Cumplimiento**     | 20+                 | Hardening SSRF, caping de credenciales, limitación de velocidad por punto de conexión, enfoque de clave de gestión |
| 📊 **Observabilidad**               | 15+                 | Integración de OpenTelemetry, seguimiento en tiempo real de cuotas, seguimiento de costos por modelo               |
| 🔄 **Integraciones de Proveedores** | 20+                 | Registros de modelo dinámico, pausas de proveedor, Codex de cuenta múltiple, parser de cuota de Copilot            |
| ⚡ **Rendimiento**                  | 15+                 | Capa de cache dual, cache de solicitud, cache de respuesta, keepalive de transmisión, API de lote                  |
| 🌐 **Ecosistema**                   | 10+                 | API de WebSocket, re carga de configuración caliente, almacenamiento de configuración distribuido, modo comercial  |

### Próximamente

- 🔗 **Integración de OpenCode** — Soporte nativo de proveedor para el IDE de
  codificación de inteligencia artificial OpenCode
- 🔗 **INTEGRACIÓN TRAE** — Compatible completo con el marco de desarrollo de
  inteligencia artificial TRAE
- 📦 **API EN LOTE** — Procesamiento de lote asíncrono para solicitudes en lotes
- 🎯 **RUTEO BASADO EN ETIQUETAS** — Rutea solicitudes en función de etiquetas y
  metadatos personalizados
- 💰 **ESTRATEGIA DE COSTO MÁS BAJO** — Selecciona automáticamente el proveedor
  más barato disponible

> 📝 Específicas de todas las características disponibles en
> [`docs/nuevas-características/`](docs/new-features/) (217 específicas
> detallados)

---

## 👥 Colaboradores

[![Colaboradores](https://contrib.rocks/image?repo=diegosouzapw/OmniRoute&max=100&columns=20&anon=1)](https://github.com/diegosouzapw/OmniRoute/graphs/contributors)

### Cómo Contribute

1. Fork el repositorio
2. Crea tu rama de características (`git checkout -b feature/amazing-feature`)
3. Haz commit de tus cambios (`git commit -m 'Agrega característica
   impresionante'`)
4. Envía el cambio al repositorio (`git push origin feature/amazing-feature`)
5. Abre una Solicitud de Actualización

Consulta [[CONTRIBUTING.md](CONTRIBUTING.md)] para detalles de las guías de
estilo.

### Publicar una Nueva Versión

```bash
# Crea una versión — npm publish sucederá automáticamente
gh release create v2.0.0 --title "v2.0.0" --generate-notes
```

---

## 📊 Histórico de estrellas

## Estrellas durante el tiempo

## [![Histórico de estrellas durante el tiempo](https://starchart.cc/diegosouzapw/OmniRoute.svg?variant=adaptive)](https://starchart.cc/diegosouzapw/OmniRoute)

## 🙏 Agradecimientos

Agradecemos especialmente a
**[CLIProxyAPI](https://github.com/decolua/9router)[X36X] por el original
proyecto que inspiró esta bifurcación. OmniRoute basa su edición en ese
impresionante fondo con características adicionales, API multimodal y una
reescritura completa en TypeScript.

Esperamos agradecer a
**[9router](https://github.com/router-for-me/CLIProxyAPI)[X32X] y
[X38X][decolua]{2}[X52X] — el original proyecto original en que se inspiró con
muchas funcionalidades que se reescribieron en el proyecto OmniRoute.

---

## 📄 Licencia

Licencia MIT - consulte [LICENSE](LICENSE) para obtener más información.

---

<div align="center">
  <sub>Built with ❤️ for developers who code 24/7</sub>
  <br/>
  <sub><a href="https://omniroute.online">omniroute.online</a></sub>
</div>
<!-- GitHub Discussions enabled for community Q&A -->
