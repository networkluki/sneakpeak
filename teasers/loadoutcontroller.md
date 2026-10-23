# PROJECT 003 // LoadoutController

**Status:** `BUILDING`  
**Platform:** Rust server · Oxide/uMod  
**Language:** C#  
**Previewed version:** `1.0.1`  
**Developer:** networkluki  
**Public preview:** 2026-10-23

> Admin UI to assign persistent per-player loadouts, given on respawn.

## 👁️ First look

A small, curated excerpt from a Rust server plugin. The snippet shows plugin metadata, selected state fields, and initialization. The complete implementation is not public.

<details>
<summary><strong>👁️ Reveal C# preview</strong></summary>

```csharp
namespace Oxide.Plugins
{
    [Info("LoadoutController", "networkluki", "1.0.1")]
    [Description("Admin UI to assign persistent per-player loadouts, given on respawn.")]
    public class LoadoutController : RustPlugin
    {
        private const string PermAdmin = "loadoutcontroller.admin";
        private const string UiRoot = "LoadoutControllerUI";

        private StoredData data;
        private ConfigData cfg;

        private readonly Dictionary<ulong, UiState> uiState = new Dictionary<ulong, UiState>();
        private readonly HashSet<ulong> givenThisLife = new HashSet<ulong>();

        #region Hooks

        private void Init()
        {
            permission.RegisterPermission(PermAdmin, this);

            LoadConfigValues();
            LoadData();
            EnsureDefaultLoadoutExists();
        }
```

</details>

## What this preview reveals

- A Rust server plugin built with C# and the Oxide plugin API.
- An admin-focused UI for persistent player loadouts.
- A glimpse of the initialization flow and per-player state.

## 🔒 Still under wraps

- Full player loadout handling and persistence implementation.
- Permission enforcement at administrative actions and UI endpoints.
- Respawn and distribution logic, validation, and full configuration.

**Note:** The provided code is intentionally truncated, including unclosed declarations. This is not a complete, compile-ready plugin or a release announcement.

*A glimpse of the control room. The rest remains behind the interface.*

[← Back to all teasers](README.md)
