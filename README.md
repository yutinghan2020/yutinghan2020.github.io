# 我的个人博客 #
现在的前端开发趋向于组件化。特别是有了Angular、React、Vue这三大框架之后，各大前端ui框架就层出不穷。这对于前端开发人员来说是好事情，可以大大提高开发效率。

这三大框架的具体说明我就不再阐述，大家可以自行去看官方文档。

[Angular文档](https://angular.cn)

[React文档](https://reactjs.org)

[Vue文档](https://cn.vuejs.org/)

现在本人使用最多的框架是VUE。所以本博客更多的是介绍vue的相关知识点。
## 简单介绍vue ##
Vue.js是一个轻巧、高性能、可组件化的MVVM库，同时拥有非常容易上手的API；

Vue.js是一个构建数据驱动的Web界面的库。

Vue.js是一套构建用户界面的 渐进式框架。与其他重量级框架不同的是，Vue 采用自底向上增量开发的设计。Vue 的核心库只关注视图层，并且非常容易学习，非常容易与其它库或已有项目整合。另一方面，Vue 完全有能力驱动采用单文件组件和 Vue 生态系统支持的库开发的复杂单页应用。数据驱动+组件化的前端开发。

**简而言之**：Vue.js是一个构建数据驱动的 web 界面的渐进式框架。Vue.js 的目标是通过尽可能简单的 API 实现响应的数据绑定和组合的视图组件。核心是一个响应的数据绑定系统。
原文链接：[https://blog.csdn.net/gao_xu_520/java/article/details/76020365](https://blog.csdn.net/gao_xu_520/java/article/details/76020365)

## 本人的项目历程 ##

在N年前，本人刚毕业出来还是一个小白的时候第一个项目用的是jquery,一个项目下来让我从一个小白成长很多，jquery的各种插件库，自定义组件封装等等。后面开始使用vue。通过对比发现vue的组件化开发比jquery在效率上提高了一个层次。首先vue的优势是它有许多的ui框架。比如Element ui、ant design vue、iView等等

智慧校园平台：[http://login.sheepdata.com](http://login.sheepdata.com) 框架（jquery）；

CRM系统：[http://crm.sheepdata.com/](http://crm.sheepdata.com/) 框架（vue）;

场地预约管理系统PC端：[http://bookui.sheepdata.com](http://bookui.sheepdata.com) 框架（vue）,微信小程序：数字小镇配套球场
## 更多 ##
### 好用的函数库、工具类--xe-utils ###

最新版本见 [Github](https://github.com/xuliangzhan/xe-utils)，点击查看[历史版本](https://github.com/xuliangzhan/xe-utils/releases)

XEUtils 提供一套实用的基础函数、任意格式的日期转换函数，浏览器相关操作函数等等

npm安装

	npm install xe-utils

全局引用

    import XEUtils from 'xe-utils'
     
    XEUtils.setup({
      cookies: {
    	path: '/'
      },
      treeOptions: {strict: false, parentKey: 'parentId', key: 'id', children: 'children', data: null},
      formatDate: 'yyyy-MM-dd HH:mm:ss.SSS',
      formatString: 'yyyy-MM-dd HH:mm:ss',
      formatStringMatchs : {
    	E: ['周日', '周一', '周二', '周三', '周四', '周五', '周六'],
    	q: [null, '第一季度', '第二季度', '第三季度', '第四季度']
      },
      commafys: {spaceNumber: 3, separator: ',', fixed: 0}
    })

	Vue.prototype.$XEUtils=XEUtils;