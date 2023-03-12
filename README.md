
# FoldTheBraces - Sublime Text Plugin
<i>This plugin is forked from the following repo:</i> https://github.com/jamalsenouci/sublimetext-syntaxfold

A plugin for Sublime Text 3 that folds/collapses or unfolds/expands code blocks contained within curly braces in haml files.

## Background
Some haml files can contain a lot of curly braces and sometimes the code within these braces can be quite long. This can make it difficult to navigate the code. This plugin was created to support the folding of code within all the curly braces in a haml file.

<i>Note: This plugin only supports haml files for now.</i>

## Installation
Clone this repository to your Sublime Text packages directory. It is usually in a path similar to this:
-   **Windows**:  `%APPDATA%\Sublime Text 3/Packages`
-   **OS X**:  `~/Library/Application Support/Sublime Text 3/Packages`
-   **Linux**:  `~/.config/sublime-text-3/Packages`


## Usage
- Use [keybindings](#key-bindings) to fold/unfold your code.

**OR** 
- Invoke fold commands through the command panel.

### Key Bindings

The following is an excerpt of the default key bindings.

<i>Note: On MacOS, the alt key is substituted with the option key.</i>

```js
[
//Fold all code blocks
  { "keys": ["alt+0", "alt+0"],
    "command": "fold_all" },

// Unfold all code blocks
  { "keys": ["alt+shift+0", "alt+shift+0"],
    "command": "unfold_all"},

// Toggle fold current code block
  { "keys": ["alt+1", "alt+1"],
    "command": "toggle_fold_current"},
]
```

### Command Reference

A list of commands have been added to the command palette and can be accessed using <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>P</kbd>.
All commands start with "FoldTheBraces : [command name]".

***Fold All***:
Fold/collapse all curly brace blocks in the current document.

***Unfold all***:
Unfold/expand all curly brace blocks in the current document.

***Toggle Fold Current***:
Folds/collapses or Unfolds/expands the curly brace block where the cursor is placed on.

***Open README***:
Open this readme file.

### Saving fold state

This plugin doesn't support saving the folded state of a file (remembering which blocks you have folded) but there is a package called BufferScroll perfectly suited to that: https://packagecontrol.io/packages/BufferScroll
