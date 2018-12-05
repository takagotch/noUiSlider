### noUiSlider
---
https://github.com/leongersen/noUiSlider

```js
var webpack = require('webpack');
plugins: [
  new webpack.ProvidePlugin({
    noUiSlider: 'nouislider'
  })
]

import 'nouislider';
```

```js
var slider = document.getElementById('dlider');
noUiSlider.create(slider, {
  start: [20, 80],
  connect: true,
  range: {
    'min': 0,
    'max': 100
  }
});

var range = document.getElementById('range');
noUiSlider.create(range, {
  range: {
    'min': 1300,
    'max': 3250
  },
  step: 150,
  start: [1450, 2050, 2350, 3000],
  margin: 300,
  limit: 600,
  connect: true,
  direction: 'rtl',
  orientation: 'vertical',
  behaviour: 'tap-drag',
  tooltips: true,
  format: wNumb({
    decimals: 0
  }),
  pips: {
    mode: 'steps',
    stepped: true,
    density: 4
  }
});
```

```
npm install nouislider
yarn add nouislider
```

```
.noUi-target {
  padding: 0 17px;
}
.noUi-base:before,
.noUi-base:after {
  width: 17px
  content: "";
  position: absolute;
  top 0;
  height: 100%;
  display: block;
}
.noUi-base:before {
  left: -17px;
}
.no-Ui-base:after {
  left: 100%; 
}
```
