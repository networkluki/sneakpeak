# PROJECT 001 // NetworkLuki Drugs

**Status:** `BUILDING`  
**Platform:** FiveM / GTA V  
**Previewed version:** `1.1.0`  
**Developer:** NetworkLuki  
**Public preview:** 2026-10-23

> Persistent, server-authoritative farming and fictional production systems.

## 👁️ First look

A curated glimpse of the resource manifest, not the full resource or an installable release. The implementation, internal logic, and undisclosed features remain private.

<details>
<summary><strong>👁️ Reveal Lua preview</strong></summary>

```lua
fx_version 'cerulean'
game 'gta5'
lua54 'yes'

name 'networkluki-drugs'
author 'NetworkLuki'
description 'Persistent, server-authoritative farming and fictional drug production systems.'
version '1.1.0'

shared_scripts {
    '@ox_lib/init.lua',
    'shared/config.lua',
    -- Other files omitted from this preview
}

server_scripts {
    'server/farming.lua',
    -- Implementation details not shown
}

client_scripts {
    'client/farming.lua',
    -- Additional modules not shown
}

dependencies {
    'ox_lib',
    'oxmysql',
    'ox_inventory',
    'ox_target'
}
```

</details>

## What this preview shows

- A FiveM resource built around Lua.
- Selected integration dependencies.
- High-level farming and fictional production themes.

## 🔒 Still under wraps

- Full source code and internal implementation.
- Data model, validation flows, and security-sensitive logic.
- Additional features and unpublished design decisions.

**Note:** This is an intentionally incomplete example. It is not intended to be copied as a working `fxmanifest.lua`.

*More when it is ready to show.*

[← Back to all teasers](README.md)
