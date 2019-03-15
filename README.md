# materialloader
JavaScript loading animation. 

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
1. Create a HTML file and include with:
```html
<script src="./materialloader-horizontal.js"></script>
```

2. Create a HTML tag `canvas`：
```html
<canvas id="canvas"></canvas>
```

3. Instantiate the JavaScript object and call function `start`:
```javascript
var loader = new HorizontalMaterialLoader(document.getElementById('canvas'));

loader.start();
```

## API
#### .init(option)
Initialize the animation optionally, and the `option` is as follows:

* HorizontalMaterialLoader
```
{
  staticCircleCount: (default: 5),
  staticCircleRadius: (default: 10),
  staticCircleRadiusScaleRate: (default: 0.4),
  fillColor: '(default: #4DB9FF)',
  duration: (default: 2000),
}
```

* RoundMaterialLoader
```
{
  bigCircleRadius: (default: 50),
  staticCircleRadiusScaleRate: (default: 0.4),
  fillColor: '(default: #4DB9FF)',
  duration: (default: 2000),
}
```

#### .start() 
Start animation.

#### .stop() 
Stop animation.
