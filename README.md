# VisualStudioCodeTweaking

After install Visual Studio Code in your PC, I use the following tweaking to its settings/preferences in a way I feel comfortable.

## Tweaking

I usually change to Tab size, word wrapping, editor width, theme, etc.

1. Minimap


## Extensions

I also install few Extension for the ease of my coding.

### 1. phpcs

### 2. Better Align: by "wwm"

There's no built-in shortcut comes with the extension, you have to add shotcuts by yourself:

Type Ctrl+Shift+p to open "Command Palette" and type "open shortcuts", OR, Press Ctrl+K+S to open "keybinding settings". A new screen comes. There is search bar at the top of this page. Below this line, there is a link saying "For advanced customizations open and edit keybindings.json". Click on the link keybindings.json.

Add something similar like this:
```
{ "key": "ctrl+alt+=",  "command": "wwm.aligncode",
    "when": "editorTextFocus && !editorReadonly"
}
```

### 3. PHP IntelliSense: by "Felix Becker"

### 4. PHP Debug: by "Felix Becker"
