---
layout: post
title: 基于jsonview插件进行chrome插件开发分析.md
description: 在做开发调试的时候，后端程序进行json输出，在谷歌浏览器打开是一大段字符串，看起来很不舒服...
key: 程序员
---

在做开发调试的时候，后端程序进行json输出，在谷歌浏览器打开是一大段字符串，看起来很不舒服，于是我就计划找一个做json展示的插件，发现了jsonview这个插件，然后谷歌的扩展程序商店无法打开，没办法，经过搜索找到jsonview的官方，然后再到gitHub上下载jsonview源代码，自己在插件管理中进行导入。也顺带编译成了谷歌插件，经过这样一个流程，也基本熟悉了chrome浏览器的插件运作模式。

## manifest.json ##

这个文件是谷歌浏览器插件的运行入口，这个文件是一个json格式的配置文件，以下我对此文件做一个说明，先附上代码：

```
{
   "content_scripts": [ { // 脚本配置
      "js": [ "jsonview.js" ], // 首先运行的js脚本
//      "css" : ["default.css"], // 这里注释掉是因为样式引入放在程序里判断在引入，不然插件只要启动就会影响正常网页样式
      "matches": [ "http://*/*", "file:///*/*" ] //这个在这里是插件内部使用的配置
   } ],
	"icons": { "48": "logo48.png",
	          "128": "logo128.png" }, // 图标资源
   "description": "Pretty-prints JSON data in the browser.", // 插件描述
   "key": "supfMA0GCSqGSIb3DQEBAQUAA4GNADCBiQKBgQDDhKAwhHMEEr5pw/QvMhtfEgh5AOX7v39DYK0l48jxvpjl2syoYsZxkC57n0nORQQh8ndLuNW8KZP4R9AkEFhXctAen28e6MKDBGg0TJaTtWkmB8Wc2sN/LNq6iJeFIebkID5TAVuqqfTpO3NOo9V+6o+bH85j8u78YOb4ZZ1U8wIDAQAB", // 这个东西我不是很清楚，应该是从谷歌开发者申请的key值
   "name": "JSONView", // 插件名称
   "version": "1.0", // 版本
   "manifest_version" : 2, // 这个不用管，必须这么设置就对了
   "web_accessible_resources" : [ // 资源加载配置，设置了才能在插件程序引入css和js等资源文件，甚至图片文件
      "/*"
   ]
}
```

关于配置说明已经在上面以注释的形式进行了说明；

具体的代码可以参考以下链接：
https://github.com/jamiew/jsonview-chrome

这上面下载下来的代码无法加载使用主要就是因为配置没有按照上面的配置，改为上面的配置就行了。