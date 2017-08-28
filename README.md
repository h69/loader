# MaterialLoader
MaterialLoader是一个基于JavaScript Canvas的加载动画库，目前提供`HorizontalMaterialLoader`等。

## Preview 
* HorizontalMaterialLoader

![HorizontalMaterialLoader](https://github.com/adamearthhuang/MaterialLoader/blob/master/screenshot/materialloader-horizontal.gif)

* RoundMaterialLoader

![RoundMaterialLoader](https://github.com/adamearthhuang/MaterialLoader/blob/master/screenshot/materialloader-round.gif)

## Usage
```html
<script src="./materialloader-xxx.js"></script>
```

## Examples
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

## API
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
    bigCircleRadius: 50,
    staticCircleRadiusScaleRate: 0.4,
    fillColor: '#4DB9FF',
    duration: 2000
}
```

#### .start() 
开始动画。

#### .stop() 
停止动画。

## License
Copyright 2017 Adamearth Huang

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

