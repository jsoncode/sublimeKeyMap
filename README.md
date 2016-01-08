# sublimeKeyMap
sublimeKeyMap and plugin

## package Control

> Package Control 插件是一个方便 Sublime text 管理插件的插件

>打开console

>>View>Show Console 或者 Ctrl+~

>>将以下 Python 代码粘贴进去并 enter 执行

>Sublime Text 3：

```
import urllib.request,os; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); open(os.path.join(ipp, pf), 'wb').write(urllib.request.urlopen( 'http://sublime.wbond.net/' + pf.replace(' ','%20')).read())
```
>Sublime Text 2：

```
import urllib2,os; pf='Package Control.sublime-package'; ipp = sublime.installed_packages_path(); os.makedirs( ipp ) if not os.path.exists(ipp) else None; urllib2.install_opener( urllib2.build_opener( urllib2.ProxyHandler( ))); open( os.path.join( ipp, pf), 'wb' ).write( urllib2.urlopen( 'http://sublime.wbond.net/' +pf.replace( ' ','%20' )).read()); print( 'Please restart Sublime Text to finish installation')
```

>手动安装方法：
>>1.点击Preferences > Browse Packages菜单

>>2.进入打开的目录的上层目录，然后再进入Installed Packages/目录

>>3.下载 Package Control.sublime-package 并复制到Installed Packages/目录

>>4.重启Sublime Text。

>>下载地址https://github.com/wbond/sublime_package_control

>然后就可以使用 Ctrl+Shift+P 安装其他插件了

### SublimeTmpl

> Ctrl+Alt+H 自动创建html模板

> CtrlAlt+J 自动创建js模板

> Ctrl+Alt+C 自动创建css模板

> Ctrl+Alt+P 自动创建php模板

> Ctrl+Alt+R 自动创建rube模板

> Ctrl+Alt+Shift+P 自动创建python模板

### HTML-CSS-JS Prettify 格式化html,css,js （需要配置nodejs安装路径）

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

### Emmet

>快速编辑，自动补全html/css的功能

### DocBlockr

>代码注释，通过解析功能，参数，变量，并且自动添加基本项目
