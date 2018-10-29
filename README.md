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
  "workbench.colorTheme": "Graphite",
  "editor.fontFamily": "SF Mono, Menlo, Monaco, 'Courier New', monospace",
  "editor.fontSize": 17,
  "editor.lineHeight": 25,
  "editor.letterSpacing": 0.5,
  "files.trimTrailingWhitespace": true,
  "editor.fontWeight": "400",
  "prettier.eslintIntegration": true,
  "editor.cursorStyle": "line",
  "editor.cursorWidth": 5,
  "editor.cursorBlinking": "solid",
  // Very important: Install this plugin: https://github.com/be5invis/vscode-custom-css
  // You'll need to change this to a file URI scheme on your computer: https://en.wikipedia.org/wiki/File_URI_scheme
  // Mac/Linux: file:///Users/YOUR-PC-USERNAME/.vscodestyles.css
  // Windows: file:///C:/Users/YOUR-PC-USERNAME/.vscodestyles.css
  "vscode_custom_css.imports": [
    "file:///Users/kd/.vscodestyles.css"
  ],
  "editor.renderWhitespace": "all",
}
```

## CSS Hacks/Overrides
1. Install [this plugin](https://github.com/be5invis/vscode-custom-css).
1. Make a file on your computer that will hold your custom CSS, `~/.vscodestyles.css`
1. Then put this everything in [graphite-custom-hacks.css](./graphite-custom-hacks.css) into your file.

Open your command palette and select enable **custom CSS and JS**

![Custom CSS/JS Hack](https://d3vv6lp55qjaqc.cloudfront.net/items/0B37352D3s2A2e33353c/Screen%20Shot%202017-09-15%20at%2011.02.49%20AM.png?X-CloudApp-Visitor-Id=26998&v=7ff79bcc)

Finally reload your editor and the Custom CSS should be taking. You can test this by typing into file - the dirty circle should be yellow not white.

**_Note: Reload custom CSS and JS after every VSCode update!_**