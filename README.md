# loader
JavaScript loading animation. 

## Preview 
* HorizontalLoader

![HorizontalLoader](./screenshot/loader-horizontal.gif)

* RoundLoader

![RoundLoader](./screenshot/loader-round.gif)

## Usage
```html
<script src="./loader-xxx.js"></script>
```

## Examples
1. Create a HTML file and include with:
```html
<script src="./loader-horizontal.js"></script>
```

2. Create a HTML tag `canvas`：
```html
<canvas id="loader"></canvas>
```

3. Instantiate the JavaScript object and call function `start`:
```javascript
var loader = new HorizontalLoader(document.getElementById('loader'));

loader.start();
```

## API
#### .init(option)
Initialize the animation optionally, and the `option` is as follows:

* HorizontalLoader
```
{
  staticCircleCount: (default: 5),
  staticCircleRadius: (default: 10),
  staticCircleRadiusScaleRate: (default: 0.4),
  fillColor: '(default: #4DB9FF)',
  duration: (default: 2000),
}
```

* RoundLoader
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
