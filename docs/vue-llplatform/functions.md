# 功能页面
本章节介绍一些常见功能的实现。

::: tip 提示
文中不会介绍详细的实现方式，各个功能的官网都有更详细的介绍。本章主要介绍功能类别以及常用插件。
:::


## 图表
【说明】

vue图表有许多选择，看个人习惯用哪一种。若图表在项目中用的地方较少，建议按需引入，不要完整引入。

本项目采用了百度的[ECharts](http://echarts.baidu.com/)，为了使用方便，引入[v-charts](https://v-charts.js.org/#/)组件（在使用 echarts 生成图表时，经常需要做繁琐的数据类型转化、修改复杂的配置项，v-charts 的出现正是为了解决这个痛点。基于 Vue2.0 和 echarts 封装的 v-charts 图表组件，只需要统一提供一种对前后端都友好的数据格式设置简单的配置项，便可轻松生成常见的图表）。

【代码示例】：[https://github.com/linjinze999/vue-llplatform/blob/master/src/pages/functions/charts/FuncCharts.vue](https://github.com/linjinze999/vue-llplatform/blob/master/src/pages/functions/charts/FuncCharts.vue)

【在线演示】：[https://linjinze999.github.io/preview/vue-llplatform/#/charts](https://linjinze999.github.io/preview/vue-llplatform/#/charts)

【预览图片】：

<img src="/assets/img/vue-llplatform/func-chart.png" />

## 表单
【说明】

[Element Form](http://element-cn.eleme.io/#/zh-CN/component/form)提供了基础的表单，如单选、多选、输入、选择、联级选择、开关、日期、文件、穿梭框、颜色选择等，参考官网使用即可。

【代码示例】：[https://github.com/linjinze999/vue-llplatform/blob/master/src/pages/functions/forms/FuncFormsBase.vue](https://github.com/linjinze999/vue-llplatform/blob/master/src/pages/functions/forms/FuncFormsBase.vue)

【在线演示】：[https://linjinze999.github.io/preview/vue-llplatform/#/forms/base](https://linjinze999.github.io/preview/vue-llplatform/#/forms/base)

【预览图片】：

<img src="/assets/img/vue-llplatform/func-form.png" />

## 富文本编辑器
【说明】

富文本编辑器可选项也较多（[常见富文本](https://panjiachen.github.io/vue-element-admin-site/zh/component/rich-editor.html)），本项目采用[vue-quill-editor](https://www.awesomes.cn/repo/surmon-china/vue-quill-editor)，其风格较为简洁。

【代码示例】：[https://github.com/linjinze999/vue-llplatform/blob/master/src/pages/functions/forms/FuncFormsEdit.vue](https://github.com/linjinze999/vue-llplatform/blob/master/src/pages/functions/forms/FuncFormsEdit.vue)

【在线演示】：[https://linjinze999.github.io/preview/vue-llplatform/#/forms/edit](https://linjinze999.github.io/preview/vue-llplatform/#/forms/edit)

【预览图片】：

<img src="/assets/img/vue-llplatform/func-edit.png" />

## 表格
【说明】

[Element Table](http://element-cn.eleme.io/#/zh-CN/component/table)提供了表格组件，加上[Element Pagination](http://element-cn.eleme.io/#/zh-CN/component/pagination)分页组件，即可完成正常的表格显示。

::: tip 提示
分页时，table需要过滤数据，只显示分页的数据，可以如此过滤：`:data="tableData.slice((currentPage-1)*pageSize,currentPage*pageSize)"`
:::

【代码示例】：[https://github.com/linjinze999/vue-llplatform/blob/master/src/pages/functions/table/FuncTable.vue](https://github.com/linjinze999/vue-llplatform/blob/master/src/pages/functions/table/FuncTable.vue)

【在线演示】：[https://linjinze999.github.io/preview/vue-llplatform/#/table](https://linjinze999.github.io/preview/vue-llplatform/#/table)

【预览图片】：

<img src="/assets/img/vue-llplatform/func-table.png" />

## 拖曳
【说明】

本项目采用了[vue.draggable](https://www.npmjs.com/package/vuedraggable)来提供拖曳功能。

【代码示例】：[https://github.com/linjinze999/vue-llplatform/blob/master/src/pages/functions/drag/FuncDrag.vue](https://github.com/linjinze999/vue-llplatform/blob/master/src/pages/functions/drag/FuncDrag.vue)

【在线演示】：[https://linjinze999.github.io/preview/vue-llplatform/#/drag](https://linjinze999.github.io/preview/vue-llplatform/#/drag)

【预览图片】：

<img src="/assets/img/vue-llplatform/func-drag.gif" />


## 其他
1. 复制粘贴：[clipboard.js](https://clipboardjs.com/)
2. excel导入导出：[vue中使用excel导入导出](https://www.cnblogs.com/liguiwang/p/8430672.html)