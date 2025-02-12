English | [简体中文](./README_CN.md)

vConsole
---
A lightweight, extendable front-end developer tool for mobile web page.

vConsole is the official debugging tool for WeChat Miniprograms.


## Features

- Logs: `console.log|info|error|...`
- Network: `XMLHttpRequest`, `Fetch`, `sendBeacon`
- Element: HTML elements tree
- Storage: `Cookies`, `LocalStorage`, `SessionStorage`
- Execute JS command manually
- Custom plugins



## Release Notes

Latest version: [![npm version](https://img.shields.io/npm/v/vconsole/latest.svg)](https://www.npmjs.com/package/vconsole)

Detailed release notes for each version are available on [Changelog](./CHANGELOG.md).



## Guide

See [Tutorial](./doc/tutorial.md) for more usage details.

For installation, there are 2 primary ways of adding vConsole to a project:

Method 1: Using npm (Recommanded)

```bash
$ npm install vconsole
```

```javascript
import VConsole from 'vconsole';

const vConsole = new VConsole();
// or init with options
const vConsole = new VConsole({ maxLogNumber: 1000 });

// call `console` methods as usual
console.log('Hello world');

// remove it when you finish debugging
vConsole.destroy();
```

Method 2: Using CDN in HTML:

```html
<script src="https://unpkg.com/vconsole@latest/dist/vconsole.min.js"></script>
<script>
  // VConsole will be exported to `window.VConsole` by default.
  var vConsole = new window.VConsole();
</script>
```



## Preview

![](./doc/snapshot/qrcode.png)

[http://wechatfe.github.io/vconsole/demo.html](http://wechatfe.github.io/vconsole/demo.html)

![](./doc/snapshot/panel_log.jpg) ![](./doc/snapshot/panel_network.jpg) ![](./doc/snapshot/panel_element.jpg) ![](./doc/snapshot/panel_storage.jpg)


## Documentation

vConsole:

 - [Tutorial](./doc/tutorial.md)
 - [Public Properties & Methods](./doc/public_properties_methods.md)
 - [Helper Functions](./doc/helper_functions.md)

Plugin:

 - [Plugin: Getting Started](./doc/plugin_getting_started.md)
 - [Plugin: Building a Plugin](./doc/plugin_building_a_plugin.md)
 - [Plugin: Event List](./doc/plugin_event_list.md)


## Third-party Plugins

 - [vConsole-sources](https://github.com/WechatFE/vConsole-sources)
 - [vconsole-webpack-plugin](https://github.com/diamont1001/vconsole-webpack-plugin)
 - [vconsole-stats-plugin](https://github.com/smackgg/vConsole-Stats)
 - [vconsole-vue-devtools-plugin](https://github.com/Zippowxk/vue-vconsole-devtools)
 - [vconsole-outputlog-plugin](https://github.com/sunlanda/vconsole-outputlog-plugin)
 - [vite-plugin-vconsole](https://github.com/vadxq/vite-plugin-vconsole)


## Feedback

QQ Group: 497430533

![](./doc/snapshot/qq_group.png)


## License

[The MIT License](./LICENSE)
