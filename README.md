### pino
---
https://github.com/pinojs/pino

```
npm install pino

cat app.log | pino-pretty -c -l
```

```js
const logger = require('pino')()

logger.info('hello')

const child = logger.child({ a: 'property' })
child.info('hello')


```

```
{"level":30,"time":xxxxxxxx,"msg":"hello","pid":657,"hostname":"Davids-MBP-3.fritz.box","v":1}
{"level":30,"time":xxxxxxxx,"msg":"hello child", "pid":657,"hostname":"Davids-MBP-3.fritz.box","a":"property","v":1}
```


