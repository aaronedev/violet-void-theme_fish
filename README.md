# Violet Void Theme - Fish

Violet Void color theme for the Fish shell.

## Installation

### Option 1: Manual Installation

```fish
# Create themes directory if it doesn't exist
mkdir -p ~/.config/fish/themes

# Symlink the theme
ln -s /path/to/violet_void.fish ~/.config/fish/themes/violet_void.fish

# Add to your fish config (~/.config/fish/config.fish)
set -g fish_theme violet_void
```

### Option 2: Clone and Link

```fish
# Clone the repository
git clone https://github.com/aaronedev/violet-void-theme_fish.git
cd violet-void-theme_fish

# Create symlink
ln -s (pwd)/violet_void.fish ~/.config/fish/themes/violet_void.fish

# Enable in config.fish
echo 'set -g fish_theme violet_void' >> ~/.config/fish/config.fish
```

## Colors

### Base Palette

| Name | Hex | Usage |
|------|-----|-------|
| `foreground` | `#c8d3f5` | Default text color |
| `selection` | `#2d3f76` | Selected text background |
| `comment` | `#636da6` | Comments and secondary text |

### Syntax Highlighting

| Name | Hex | Usage |
|------|-----|-------|
| `red` | `#ff757f` | Errors |
| `orange` | `#ff966c` | End of command block |
| `yellow` | `#ffc777` | Strings and quotes |
| `green` | `#c3e88d` | Operators |
| `cyan` | `#86e1fc` | Commands |
| `purple` | `#fca7ea` | Parameters and variables |
| `pink` | `#c099ff` | Keywords |
| `foreground` | `#c8d3f5` | Normal text, redirections |

### Pager Colors

| Name | Hex | Usage |
|------|-----|-------|
| `progress` | `#636da6` | Progress indicator |
| `prefix` | `#86e1fc` | Prefix/highlighted item |
| `completion` | `#c8d3f5` | Completed items |
| `description` | `#636da6` | Item descriptions |

## Configuration Tips

### Enable/Disable Components

```fish
# Disable search match highlighting
set -g fish_color_search_match

# Use a different comment color
set -g fish_color_comment 828bb8
```

### Custom Pager Styling

```fish
# Brighter pager prefix
set -g fish_pager_color_prefix 00bcff

# Highlighted row background
set -g fish_pager_color_selected_background --background=2d3f76
```

## License

[MIT](https://opensource.org/licenses/MIT)

Part of the [Violet Void](https://github.com/aaronedev/violet-void-monorepo) theme ecosystem.
