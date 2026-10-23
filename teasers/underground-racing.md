# PROJECT 002 // Underground Racing

**Status:** `BUILDING`  
**Platform:** FiveM / GTA V · ESX  
**Previewed version:** `1.0.0`  
**Developer:** networkluki  
**Public preview:** 2026-10-23

> Underground racing ecosystem for ESX.

## 👁️ First look

A limited look at the Lua resource manifest and its browser-based interface. This is a curated preview, not the complete manifest or an installable release.

<details>
<summary><strong>👁️ Reveal Lua preview</strong></summary>

```lua
fx_version 'cerulean'
game 'gta5'

author 'networkluki'
description 'Underground racing ecosystem for ESX'
version '1.0.0'

lua54 'yes'

ui_page 'web/index.html'

shared_scripts {
    '@ox_lib/init.lua',
    'config.lua'
}

client_scripts {
    'client/main.lua',
    -- Additional client modules not shown
}

server_scripts {
    '@oxmysql/lib/MySQL.lua',
    'server/main.lua',
    -- Additional server modules not shown
}

files {
    'web/index.html',
    'web/style.css',
    'web/app.js'
}

dependencies {
    'ox_lib',
    'oxmysql',
    'es_extended'
}
```

</details>

## What this preview reveals

- A racing-focused FiveM project with ESX integration.
- A Lua resource connected to a web-based user interface.
- Selected dependency and manifest declarations.

## 🔒 Still under wraps

- Server-side implementation and internal modules.
- Database schema, validation rules and operational details.
- Full gameplay mechanics and unannounced features.

**Note:** The manifest excerpt intentionally omits files and is not a deployable `fxmanifest.lua`. No release date is implied.

*Only fragments are visible. The rest stays in the garage.*

[← Back to all teasers](README.md)
