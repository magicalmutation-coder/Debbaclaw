# Debbaclaw

## OpenClaw in Termux (same UI layout)

This repository now defines Debbiebot running on an **OpenClaw backend inside Termux** while keeping the **existing screen layout and interface unchanged**.

### Required behavior

1. **Runtime backend**
   - Run OpenClaw services in Termux.
   - Debbiebot UI connects to OpenClaw adapters instead of changing UI structure.

2. **UI compatibility (no layout changes)**
   - Keep current screens and visual layout exactly as-is.
   - Keep existing:
     - Chat screen
     - Robot screen
     - Settings screen

3. **Structured control channels**
   - Add/keep structured integration for:
     - Email
     - WhatsApp
   - Both channels must support control actions and normal use flows via OpenClaw adapters.

4. **Skills and memory source**
   - Skills and memory are populated from OpenClaw stores/providers.
   - UI should consume those capabilities through the same interface contracts.

5. **Settings extensibility**
   - Settings page is the place to:
     - Configure OpenClaw connection/runtime options.
     - Enable/disable integrations.
     - Add plugins.
