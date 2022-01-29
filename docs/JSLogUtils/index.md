# JSLogUtils

A library that makes logging look better!

## Installion

Install the library:

```bash
$ npm install jslogutils
# or
$ yarn add jslogutils
```

Import the library:
```js
const JSLogUtils = require('JSLogUtils');
const logger = new JSLogUtils();
```

## Examples

Simple logging:
```js
logger.error('error');
logger.debug('debug');
logger.info('info');
logger.warning('warning');
```

Logging with prefix:
```js
logger.setPrefix(JSLogUtils.PREFIX.ERROR, '[ERROR]');
logger.setPrefix(JSLogUtils.PREFIX.DEBUG, '[DEBUG]');
logger.setPrefix(JSLogUtils.PREFIX.INFO, '[INFO]');
logger.setPrefix(JSLogUtils.PREFIX.WARNING, '[WARNING]');
```