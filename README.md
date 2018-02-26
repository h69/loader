# Ah.js

## Ah.js 是什么
Ah.js 是一个构建用户界面的自动化 JavaScript 引擎，采用自底向上增量开发的设计，它只关注视图层，不仅易于上手，还便于与第三方库或既有项目整合，令开发者无需过多关注 JavaScript 业务逻辑实现即可快速开发，如同 **「Ah」** 这个英文单词令人惊叹一般。

当然，我们希望你在使用的时候可以配合 [Bootstrap](http://www.bootcss.com/) 和 [iBootstrap](http://www.ibootstrap.cn/)，众所周知，Bootstrap 优化了 HTML、CSS 的使用，而 Ah.js 则优化了 JavaScript 的使用。

比如，这个网站就是使用 Bootstrap 和 Ah.js 构建而成的，它没有使用多余的 JavaScript 代码。

## 起步
> 官方指南假设你已了解关于 HTML、CSS 和 JavaScript 的初级知识。之前有其它框架的使用经验会有帮助，但这不是必需的。

你可以先创建一个 HTML 文件，然后通过如下方式引入 Ah.js 即可开始你的惊叹之旅：
```html
<script src="ah.js"></script>
```

然后，直接在 HTML 标签上使用 `ah-*` 属性即可完成各种 JavaScript 操作。

## # launcher
启动器引擎。

| 属性                | 说明            |
| ------------------- | -------------- |
| ah-role             | 引擎角色        |
| ah-url              | 请求地址        |
| ah-data-bind        | 请求参数数据绑定 |
| ah-callback-success | 请求成功回调     |

```html
<div ah-role="launcher" ah-url="./getData"></div>
```

## # popup
弹窗引擎。

| 属性                | 说明        |
| ------------------- | ---------- |
| ah-role             | 引擎角色    |
| ah-event-bind       | 点击事件绑定 |
| ah-animate          | 是否开启动画 |

```html
<div ah-role="popup" ah-event-bind="#popup" ah-animate="true"></div>
```

## # link
链接引擎。

| 属性                | 说明            |
| ------------------- | -------------- |
| ah-role             | 引擎角色        |
| ah-url              | 请求地址        |
| ah-target           | 响应数据目标组件 |
| ah-callback-success | 请求成功回调     |
| ah-data-bind        | 请求参数数据绑定 |

```html
<div ah-role="link" ah-url="./getData" ah-target="#link-display"></div>
```

## # button
按钮引擎。

| 属性                | 说明            |
| ------------------- | -------------- |
| ah-role             | 引擎角色        |
| ah-url              | 请求地址        |
| ah-callback-success | 请求成功回调     |
| ah-data-bind        | 请求参数数据绑定 |

```html
<div ah-role="button" ah-url="./getData" ah-callback-success="alert($data.code);"></div>
```

## # select
下拉框引擎。

| 属性                | 说明            |
| ------------------- | -------------- |
| ah-role             | 引擎角色        |
| ah-url              | 请求地址        |
| ah-callback-success | 请求成功回调     |

```html
<select ah-role="select" ah-url="./getData"></select>
```

## # table
表格引擎。

| 属性                | 说明            |
| ------------------- | -------------- |
| ah-role             | 引擎角色        |
| ah-url              | 请求地址        |
| ah-data-bind        | 请求参数数据绑定 |
| ah-event-bind       | 请求事件绑定     |
| ah-first-load       | 是否首次加载 |
| ah-callback-success | 请求成功回调     |

```html
<table ah-role="table" ah-url="./table" ah-data-bind="#date" ah-event-bind="#load"></table>
```

## 准备好了吗
我们刚才介绍了 Ah.js 最核心的基本功能 —— Ah.js 还正在完善开发中，后续会继续添加功能！

## License
Copyright 2018 Adamearth Huang

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.