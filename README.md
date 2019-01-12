# VisualStudioCodeTweaking

After install Visual Studio Code in your PC, I use the following tweaking to its settings/preferences in a way I feel comfortable.

## Tweaking

I usually change to Tab size, word wrapping, editor width, theme, etc.

1. Minimap


## Extensions

I also install few Extension for the ease of my coding.

### 1. phpcs

### 2. Better Align - by "wwm"

There's no built-in shortcut comes with the extension, you have to add shotcuts by yourself:

Type Ctrl+Shift+p to open "Command Palette" and type "open shortcuts", OR, Press Ctrl+K+S to open "keybinding settings". A new screen comes. There is search bar at the top of this page. Below this line, there is a link saying "For advanced customizations open and edit keybindings.json". Click on the link keybindings.json.

Add something similar like this:
```
{ "key": "ctrl+alt+=",  "command": "wwm.aligncode",
    "when": "editorTextFocus && !editorReadonly"
}
```

### 3. Better Comments - by Aaron Bond

### 4. PHP IntelliSense - by "Felix Becker"

### 5. PHP Debug: by "Felix Becker"

### 6. WordPress Snippet

This VSCode plugin is maintained by TungVN.

# How to update VisualStudio Code

1. Un-install VisualStudio Code.
2. Download **NEW** version and **Re-install** VisualStudio Code.

### User Settings

In Visual Studio Code editor, click File -> Preferences -> Settings. In this page, find a link "Edit in settings.json" and paste the following settings.

```js
"editor.wordWrap": "on",
"php.executablePath": "/opt/lampp/bin/php"
"php.validate.executablePath": "/opt/lampp/bin/php"
```

### Fix "Code Runner" Error in PHP

There is an extension in VS Code named, "Code Runner". I can run JS, PHP, etc. code from inside VS Code. While running PHP code file, it gives "/bin/sh: php: command not found". There is a nice explanation in StackOverflow website (https://stackoverflow.com/questions/43009623/php-command-not-found).

```
Whenever you install XAMPP, you get all of the Apache, MySQL, PHP stack. The problem is, XAMPP won't link binaries to your PATH, because your could have another version of that software already installed.

Composer needs a PHP version available on your PATH, so the easier option is to link your already installed version of PHP.

I think you can find your PHP binary in /opt/llamp/bin so you can link it this way:

sudo ln -s /opt/llamp/bin/php /usr/bin/php

Hope it works!
```
