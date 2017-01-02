# jQuery-element-move

[![GitHub release](https://img.shields.io/github/release/ben182/jQuery-element-move.svg)]()
[![Bower](https://img.shields.io/bower/v/jQuery-element-move.svg)](https://github.com/ben182/jQuery-element-move)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://paypal.me/bbortels)
[![Gitter](https://img.shields.io/gitter/room/jQuery-element-move/Stardust.svg)](https://gitter.im/jQuery-element-move/Lobby?utm_source=share-link&utm_medium=link&utm_campaign=share-link)

jQuery-element-move is a simple jQuery plugin, that allows you to make HTML elements movable. This works in any browser, including mobile touch events.

## Demo and docs
Check out: https://ben182.github.io/jQuery-element-move

## How to use?
### Bower
```
bower install jQuery-element-move
```

### Old traditional way
jQuery-element-move depends on jQuery. Include them both in end of your HTML code:
```
<script
  src="https://code.jquery.com/jquery-3.1.1.min.js"
  integrity="sha256-hVVnYaiADRTO2PzUGmuLJr8BLUSjGIZsDYGmIJLv2b8="
  crossorigin="anonymous"></script>
<script>
// To use with default settings
$('#container').elementMove();

// To use with customized settings (only allowing y-axis moving)
$('#container').elementMove({
  swipeDirection: 1
});
</script>
```

##Options
| Name | Description | Type | Default |
|------|-------------|------|---------|
| `backToOrigin` | if true, element will return to start position after release. | Boolean | false |
| `backToOriginAnimation` | A CSS transition effect is used for this effect so you can control the animation here. | String | `cubic-bezier(0.39, 0.58, 0.54, 1.42)` |
| `backToOriginAnimationDuration` | Control the animation time. | Number | 0.5 |
| `swipeDirection` | Customize the Direction of moving. 0 => only x-axis, 1 => only y-axis, 2 => full movement, 3 => only upwards, 4 => only downwards, 5 => only to the right, 6 => only to the left. | Number | 2 |
| `momentum` | You can enable momentum movement. If so, the element will move very fluid and gets extra movement based on previous acceleration afterwords. | Boolean | false |
| `stayInElement` | Your element will not move out of this. | String | false |
| `xScrollAmount` | You are able to specify a percantage of the element. When you scroll past this value on the x-axis, `scrollAmountCallback` will fire. | Number | 1 |
| `yScrollAmount` | You are able to specify a percantage of the element. When you scroll past this value on the y-axis, `scrollAmountCallback` will fire. | Number | 1 |
| `scrollAmountCallback` | Already explained above. Parameters: this. | Callback Function |  |
| `moveCallback` | Callback Function that fires when the element moves. Parameters: this, xPos(gives the pixel offset on x-axis to the start position), yPos(gives the pixel offset on y-axis to the start position). | Callback Function |  |
| `endCallback` | Callback Function that fires when you release the element. Parameters: this, xPos(gives the pixel offset on x-axis to the start position), yPos(gives the pixel offset on y-axis to the start position). | Callback Function |  |



##License

Distributed under the MIT license.

##Buy me a coffee
[Donate](https://ko-fi.com/A6749M1)

##Contact me

Feel free to contact me on Twitter [@beno182](https://twitter.com/beno182)
