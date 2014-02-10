Nirvana
=======

####基础库:

#####[mod.js](https://github.com/fouber/mod)

一个简洁的模块管理器. 所有模块都基于 define require 管理.

#####[Zepto.js](https://github.com/madrobby/zepto)

一个简洁的基础库，实现了jQuery的大部分接口. Nirvana除包括了标准Zepto.js库外，还加载了其 callback.js deferred.js touch.hs data.js 几个模块.

####模块:

##### [require('nv:util')](modules/util)

提供一些基础库不具备的功能,后期可能发展为替代Zepto.js.

##### [require('nv:app')](modules/app)

webapp核心模块,整个webapp的开发都是围绕着app进行的.

##### [require('nv:api')](modules/api)

提供web与client交互的接口注册和调用功能.

##### [require('nv:url')](modules/url)

提供url跳转和替换等功能.

##### [require('nv:view')](modules/view)

提供webapp视图管理功能.

##### [require('nv:router')](modules/router)

提供webapp地址路由功能.

##### [require('nv:style')](modules/style)

提供webapp样式管理功能.

##### [require('nv:tmpl')](modules/tmpl)

为webapp的js模板提供支持.

####依赖Zepto的模块

##### [require('nv:cache')](modules/cache)

提供数据缓存功能. 依赖Zepto.js的Deferred功能

##### [require('nv:directive')](modules/directive)

为webapp提供HTML指令功能