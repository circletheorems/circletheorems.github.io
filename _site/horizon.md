Below is a calculator that automatically calculates the distance to the horizon. The only value you need to input is your height relative to sea level (in meters). It does all the trigonometry calculations for you!

<iframe src="https://jscalc.io/embed/yeqfVAvPbM26JS4Q" width="830" height="500" frameborder="0" marginheight="0" marginwidth="0" style="border: 1px solid rgba(0,0,0,0.12)"></iframe>

## [](#header-2)Source code:

```js
'use strict';

var radian = Math.acos(inputs.radius / ((inputs.height/1000) + inputs.radius));
var angle = radian * (180 / Math.PI);
var distance = Math.tan(radian) * inputs.radius;

return {
  angle: angle,
  distance: distance
};
```
