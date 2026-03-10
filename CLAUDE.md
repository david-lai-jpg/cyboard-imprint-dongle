# Project Instructions

## Key Positions Reference

When the user references key positions by number, **always read `KEY_POSITIONS.svg`** at the project root to understand which physical key they're referring to. Do not guess positions from the keymap array alone.

## Keymap Changes

After ANY edit to `config/imprint_dongle.keymap`, **always re-render the keymap-drawer**:

1. `keymap -c keymap_drawer.config.yaml parse -z config/imprint_dongle.keymap -o keymap-drawer/imprint_dongle.yaml`
2. `keymap -c keymap_drawer.config.yaml draw -j config/imprint_dongle.json -l imprint_function_row_full_bottom_row keymap-drawer/imprint_dongle.yaml -o keymap-drawer/imprint_dongle.svg`

This is non-negotiable. Every keymap edit must be followed by both commands.
