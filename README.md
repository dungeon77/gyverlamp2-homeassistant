# Gyver Lamp 2 Integration for Home Assistant

[![hacs_badge](https://img.shields.io/badge/HACS-Custom-orange.svg)](https://github.com/hacs/integration)

Custom integration for controlling Gyver Lamp 2 devices in Home Assistant via UDP protocol.

## Features

- ✅ **Full device control** - Power on/off, brightness, effects
- ✅ **Preset management** - Create, edit, delete presets
- ✅ **Group support** - Control multiple lamps in groups
- ✅ **Real-time settings** - Live configuration updates
- ✅ **Diagnostic sensors** - Port, commands, preset info
- ✅ **Auto-discovery** - Easy setup via config flow

## Installation

### HACS (Recommended)
1. Open HACS in your Home Assistant
2. Go to "Integrations"
3. Click "+" and add this repository
4. Search for "Gyver Lamp 2" and install
5. Restart Home Assistant

### Manual Installation
1. Copy the `gyver_lamp2` folder to `custom_components` in your Home Assistant config directory
2. Restart Home Assistant
3. Add integration via Settings → Devices & Services → Add Integration

## Configuration

1. Go to Settings → Devices & Services → Add Integration
2. Search for "Gyver Lamp 2"
3. Enter your lamp details:
   - **IP Address**: Your network broadcast IP (e.g., 192.168.1.)
   - **Network Key**: Default is "GL"
   - **Group Number**: 1-8
   - **Device Name**: Custom name for your lamp

## Supported Entities

### Control
- Light (on/off)
- Preset selection
- Previous/Next preset buttons
- Group selection

### Settings
- Brightness control
- Effect selection
- Palette selection
- Speed/Scale controls
- Audio reaction settings
- Matrix configuration

### Diagnostics
- Port number
- Last command sent
- Current preset
- Presets count
- Timezone

## Protocol

The integration uses UDP broadcast protocol:
- **Type 0**: Device control commands
- **Type 1**: Settings configuration  
- **Type 2**: Presets management

## Support

- **Issues**: [GitHub Issues](https://github.com/dungeon77/gyverlamp2-homeassistant/issues)
- **Discussions**: [GitHub Discussions](https://github.com/dungeon77/gyverlamp2-homeassistant/discussions)

## License

MIT License - see LICENSE file for details
