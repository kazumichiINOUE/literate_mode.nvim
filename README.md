# SPLITE

*SPLITE spreads your coding perspectives in Literate Programming*

Neovim plugin for enhanced literate programming with spread view code display 
and dynamic syntax highlighting modes.

## Features

- **Spread View**: Multi-pane spread display for continuous code reading
- **Literate Mode**: Toggle between code-focused and documentation-focused views
- **Enhanced Comments**: Markdown-style formatting within code comments
- **Multi-language Support**: Dynamic syntax highlighting for multiple languages
- **Seamless Integration**: Simple keymap-based mode switching

## Installation

### Using [lazy.nvim](https://github.com/folke/lazy.nvim)

```lua
{
  "kazumichiINOUE/splite.nvim",
  config = function()
    require("splite").setup()
  end
}
```

<!--
### Using [packer.nvim](https://github.com/wbthomason/packer.nvim)

```lua
use {
  "kazumichiINOUE/splite.nvim",
  config = function()
    require("splite").setup()
  end
}
```
-->

## Usage

### Default Keymaps

- `<leader>lt` - Toggle literate mode
- `<leader>lv` - Toggle spread view

### Commands

- `:SpliteToggle` - Toggle literate mode
- `:SpliteSpread` - Toggle spread view mode

## Supported Languages in Literate Mode

| Language | Status | Features |
|----------|--------|----------|
| Rust     | ✅     | Full Markdown support, Headers, Bold/Italic, Code blocks, Lists |
| Python   | ✅     | Full Markdown support, Headers, Bold/Italic, Code blocks, Lists |
| Lua      | ✅     | Full Markdown support, Headers, Bold/Italic, Code blocks, Lists |
| C/C++    | 🚧     | Planned |

## Configuration

```lua
require("splite").setup({
  -- Configuration options will be added in future versions
})
```

## License

MIT
