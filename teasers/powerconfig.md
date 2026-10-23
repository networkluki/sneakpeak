# PROJECT 004 // PowerConfig

**Status:** `BUILDING`  
**Platform:** Rust server · Oxide/uMod  
**Language:** C#  
**Previewed version:** `1.1.0`  
**Developer:** networkluki  
**Public preview:** 2026-10-23

> Configures Solar Panel and Test Generator power output via JSON config.

## 👁️ First look

A curated code glimpse from the plugin's configuration model, including JSON properties and default values. No full implementation or deployable plugin is included.

<details>
<summary><strong>👁️ Reveal C# preview</strong></summary>

```csharp
namespace Oxide.Plugins
{
    [Info("PowerConfig", "networkluki", "1.1.0")]
    [Description("Configures Solar Panel and Test Generator power output via JSON config.")]
    public class PowerConfig : RustPlugin
    {
        // ─────────────────────────────────────────────
        //  Configuration
        // ─────────────────────────────────────────────

        private Configuration _config;

        private class Configuration
        {
            [JsonProperty("Solar Panel Power Output (watts)")]
            public int SolarPanelPower { get; set; } = 10000;

            [JsonProperty("Test Generator Power Output (watts)")]
            public int TestGeneratorPower { get; set; } = 100000;
        }
```

</details>

## What this preview reveals

- A C# Oxide plugin configuration structure for Rust servers.
- JSON-configurable power output for a Solar Panel and Test Generator.
- Selected default values, provided in the excerpt above.

## 🔒 Still under wraps

- Runtime behavior and application of configuration values.
- Full validation, hooks, command handling, and error paths.
- Remaining plugin implementation and deployment details.

**Note:** This is the incomplete source excerpt provided for the preview; it is not compile-ready and does not establish that the behavior is implemented or tested.

*Some of the power is visible. The whole system isn't.*

[← Back to all teasers](README.md)
