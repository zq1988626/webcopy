# webcopy

## install
```
npm install webcopy
```

## example
```js
const open = require('open');
const path = require('path');
const webcopy = require("./webcopy");
webcopy.createService('http://ramda.cn/',{
    path:path.join(__dirname,"cache/ramda")
},function(url){
    open("http://"+url,["chrome"])
})
```