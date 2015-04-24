# analytics.js-loader

This is the [segment.com snippet](https://segment.com/docs/libraries/analytics.js/quickstart/#step-1-copy-the-snippet) as a module.

*Slightly* modified to be [browserify](http://browserify.org/) compatible.

## Install

```shell
npm install analytics.js-loader --save
```

## Usage

```js
require('analytics.js-loader')({
  writeKey: 'YOUR_WRITE_KEY',
  // you can skip the first analytics.page() call if needed, #1
  skipPageCall: false
});

global.analytics.identify('1e810c197e', {
  name: 'Bill Lumbergh',
  email: 'bill@initech.com'
});

global.analytics.track('Signed Up', {
  plan: 'Startup',
  source: 'Analytics Academy'
});
```
