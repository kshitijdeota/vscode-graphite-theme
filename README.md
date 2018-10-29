# Graphite Theme for VS Code

[![Version](https://vsmarketplacebadge.apphb.com/version/kdpixels.graphite.svg)](https://marketplace.visualstudio.com/items?itemName=kdpixels.graphite)

![Preview](https://raw.githubusercontent.com/kshitijdeota/vscode-graphite-theme/master/images/ss.png)

# Installation
1. Open **Extensions** sidebar panel in VS Code. `View → Extensions`
2. Search for `Graphite` - by **KD Pixels**
3. Click **Install** to install it.
4. Click **Reload** to reload the your editor
5. Code > Preferences > Color Theme > **Graphite**
6. Optional: Use the recommended settings below for best experience

## Recommended Settings

```js
{
  "editor.cursorBlinking": "phase",
  "editor.cursorWidth": 10,
  "editor.detectIndentation": false,
  "editor.fontFamily": "SF Mono",
  "editor.fontLigatures": true,
  "editor.fontSize": 17
  "editor.lineHeight": 25,
  "editor.minimap.maxColumn": 80,
  "editor.renderWhitespace": "all",
  "editor.rulers": [80],
  "editor.tabCompletion": "on",
  "editor.tabSize": 2,
  "editor.wordWrap": "on",
  "explorer.confirmDelete": false,
  "explorer.confirmDragAndDrop": false,
  "files.trimTrailingWhitespace": true,
  "files.exclude": {
    "**/.vscode": true,
    "**/node_modules": true,
    "**/package-lock.json": true
  },
  "markdown.preview.fontSize": 15,
  "markdown.preview.lineHeight": 2.1,
  "prettier.eslintIntegration": true,
  "terminal.integrated.env.osx": {
    "PATH": "/fake/path:${env:PATH}"
  },
  "terminal.integrated.fontSize": 15,
  // Very important: Install this plugin: https://github.com/be5invis/vscode-custom-css
  // you'll need to change this to an absolute path on your computer
  "vscode_custom_css.imports": [
    "file:///Users/kd/.vscodestyles.css"
  ],
  "window.zoomLevel": 0,
  "workbench.editor.showTabs": true,
  "workbench.fontAliasing": "auto",
}
```

## CSS Hacks/Overrides
1. Install [this plugin](https://github.com/be5invis/vscode-custom-css).
1. Make a file on your computer that will hold your custom CSS, `~/.vscodestyles.css`
1. Then put this everything in [graphite-custom-hacks.css](https://raw.githubusercontent.com/kshitijdeota/vscode-graphite-theme/master/graphite-customhacks.css) into your file.

Open your command palette and select enable **custom CSS and JS**

![Custom CSS/JS Hack](https://raw.githubusercontent.com/kshitijdeota/vscode-graphite-theme/master/images/styles.png)

Finally reload your editor and the Custom CSS should be enabled. You can test this by typing into file - the dirty circle should be blue not white.

**_Note: Reload custom CSS and JS after every VSCode update!_**