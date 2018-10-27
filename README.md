# Graphite Theme for VS Code

[![Version](https://vsmarketplacebadge.apphb.com/version/wesbos.theme-cobalt2.svg)](https://marketplace.visualstudio.com/items?itemName=wesbos.theme-cobalt2)

![Preview](https://raw.githubusercontent.com/kshitijdeota/vscode-graphite-theme/master/images/ss.png)

# Installation

1. Open **Extensions** sidebar panel in VS Code. `View → Extensions`
2. Search for `Graphite` - by **KD Pixels**
3. Click **Install** to install it.
4. Click **Reload** to reload the your editor
5. Code > Preferences > Color Theme > **Cobalt2**
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
    "file:///Users/wesbos/.vscodestyles.css"
  ],
  "editor.renderWhitespace": "all",
}
```

## Important: CSS Hacks For Extra Sweet Editor
Some things in VS Code can't be controlled by settings, but you can install [this plugin](https://github.com/be5invis/vscode-custom-css), then make a file on your computer that will hold your custom CSS, I like to make one in my root called `~/.vscodestyles.css` and then put this everything in [graphite-custom-hacks.css](./graphite-custom-hacks.css) into your file.

Once done, open your command palette and select enable **custom CSS and JS**

![Custom CSS/JS Hack](https://d3vv6lp55qjaqc.cloudfront.net/items/0B37352D3s2A2e33353c/Screen%20Shot%202017-09-15%20at%2011.02.49%20AM.png?X-CloudApp-Visitor-Id=26998&v=7ff79bcc)

Finally reload your editor and the Custom CSS should be taking. You can test this by typing into file - the dirty circle should be yellow not white.

**_Note: Reloading custom CSS and JS after every VSCode update is a must!_**

## Contributing
This is a bit weird, but to get some sort of live feedback for when editing a theme. Please let me know if you have a saner way of doing it

1. Open this repo in your terminal and type `npm install`
1. Start to watch for change on the repo with `npm start` - this runs a nodemon task for you and will automatically recompile any changes
1. Open this repo in VS Code
1. Open your command palette and hit type **VSIX**. Select the one that says **Extensions: Install from VSIX...**
1. Load the VSIX file that was created a few steps back
1. Set your editor to use _this_ Cobalt2 theme - it might help to change the name in package.json to something like "Cobalt2 Dev" so you can differentiate from the Cobalt2 you've installed from the marketplace. If you get confused, just delete all traces of Cobalt2 and then load the VSIX.
1. Go to the debug sidebar `View → Debug`
1. Press the green arrow beside "Launch Extension"
1. This will then open a second window.
1. Make a change, and then hit the refresh button on your debug toolbar - this is in your first editor - not the one that poped open.
1. Wait a sec, your changes should now be reflected!