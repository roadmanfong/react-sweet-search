# react-sweet-search

[react-sweet-search](https://www.npmjs.com/package/react-sweet-search) as React components

[![NPM](https://nodei.co/npm/react-sweet-search.png)](https://www.npmjs.com/package/react-sweet-search)

## Description
React based component Search. Enhance user experience of search.


## Preview
![alt tag](https://cloud.githubusercontent.com/assets/429250/14410807/5a3a68fc-ff6a-11e5-928a-e07914dd7674.gif)


## Installation

Install via [npm](https://www.npmjs.com/package/react-sweet-search)

Step 1:
```shell
npm install --save react-sweet-search
```

Step 2:
* include node_module/react-sweet-search/dist/css/SweetSearch.css


## Usage

```js
import React from 'react';
import ReactDOM from 'react-dom';

import SweetSearch from "react-sweet-search";


const searchFn = function(inputValue, endSearch) {
  console.log('inputValue: ' + inputValue);

  endSearch();
}

const cancelFn = function (endSearch) {
  // always needs to cancel searching

  endSearch();
}

ReactDOM.render(
  <div>
    <SweetSearch search={searchFn} cancel={cancelFn} />
  </div>,
  document.getElementById("react")
);
```


## Author

smallma(s.rain@yahoo.com.tw)


## License

MIT
