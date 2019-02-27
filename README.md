# materialloader
materialloader 是一个基于 JavaScript canvas 的加载动画库，目前提供`HorizontalMaterialLoader`、`RoundMaterialLoader`等。

## 预览 
* HorizontalMaterialLoader

![HorizontalMaterialLoader](https://github.com/adamearthhuang/MaterialLoader/blob/master/screenshot/materialloader-horizontal.gif)

* RoundMaterialLoader

![RoundMaterialLoader](https://github.com/adamearthhuang/MaterialLoader/blob/master/screenshot/materialloader-round.gif)

## 起步
```html
<script src="./materialloader-xxx.js"></script>
```

## 范例
1. 引入JavaScript文件：
```html
<script src="./materialloader-horizontal.js"></script>
```

2. 在HTML页面中添加相对应的`canvas`标签：
```html
<canvas id="canvas"></canvas>
```

3. 编写JavaScript代码，创建实例后直接调用`start`函数即可：
```javascript
var loader = new HorizontalMaterialLoader(document.getElementById('canvas'));

loader.start();
```

## 方法
#### XxxMaterialLoader(canvas) 
创建实例，其中，`canvas`是DOM对象。

#### .init(option)
初始化参数（也可以不进行初始化，那么将使用默认参数），其中，`option`的结构如下：

* HorizontalMaterialLoader
```javascript
{
    staticCircleCount: 静态圆数量，默认为5
    staticCircleRadius: 静态圆半径，默认为10
    staticCircleRadiusScaleRate: 静态圆半径变化比率，默认为0.4
    fillColor: 画笔填充颜色，默认为'#4DB9FF'
    duration: 动画持续时间（毫秒），默认为2000
}
```

* RoundMaterialLoader
```javascript
{
    bigCircleRadius: 大圆半径，默认为50
    staticCircleRadiusScaleRate: 静态圆半径变化比率，默认为0.4
    fillColor: 画笔填充颜色，默认为'#4DB9FF'
    duration: 动画持续时间（毫秒），默认为2000
}
```

#### .start() 
开始动画。

#### .stop() 
停止动画。
