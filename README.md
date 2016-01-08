# sublimeKeyMap
sublimeKeyMap and plugin

>Ctrl+Shift+P 安装插件

#### SublimeTmpl

> Ctrl+Alt+H 自动创建html模板

> CtrlAlt+J 自动创建js模板

> Ctrl+Alt+C 自动创建css模板

> Ctrl+Alt+P 自动创建php模板

> Ctrl+Alt+R 自动创建rube模板

> Ctrl+Alt+Shift+P 自动创建python模板

#### HTML-CSS-JS Prettify 格式化html,css,js （需要配置nodejs安装路径）

> 配置node
>> Package Settings>HTML/CSS/JS Prettify>Set `node` Path

```
{
  // Simply using `node` without specifying a path sometimes doesn't work :(
  // https://github.com/victorporof/Sublime-HTMLPrettify#oh-noez-command-not-found
  // http://nodejs.org/#download
  "node_path": {
    "windows": "C:/Program Files/nodejs/node.exe",
    "linux": "/usr/bin/nodejs",
    "osx": "/usr/local/bin/node"
  },

  // Automatically format when a file is saved.
  "format_on_save": false,

  // Only format the selection if there's one available.
  "format_selection_only": true,

  // Log the settings passed to the prettifier from `.jsbeautifyrc`.
  "print_diagnostics": true
}
```

> Ctrl+Shift+D 代码格式化
