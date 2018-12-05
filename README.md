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
```

```
npm install nouislider
yarn add nouislider
```

