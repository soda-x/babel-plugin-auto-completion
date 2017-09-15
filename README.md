[![NPM version](https://img.shields.io/npm/v/babel-plugin-auto-completion.svg?style=flat)](https://npmjs.org/package/babel-plugin-auto-completion) [![Build Status](https://travis-ci.org/pigcan/babel-plugin-auto-completion.svg?branch=master)](https://travis-ci.org/pigcan/babel-plugin-auto-completion) [![Build status](https://ci.appveyor.com/api/projects/status/sk8hs3985idxm721/branch/master?svg=true)](https://ci.appveyor.com/project/pigcan/babel-plugin-auto-completion/branch/master) [![Coverage Status](https://coveralls.io/repos/github/pigcan/babel-plugin-auto-completion/badge.svg?branch=master)](https://coveralls.io/github/pigcan/babel-plugin-auto-completion?branch=master) [![Dependency Status](https://david-dm.org/pigcan/babel-plugin-auto-completion.svg)](https://david-dm.org/pigcan/babel-plugin-auto-completion) [![Greenkeeper badge](https://badges.greenkeeper.io/pigcan/babel-plugin-auto-completion.svg)](https://greenkeeper.io/)

# babel-plugin-auto-completion

> Babel Plugin for autopletion.

Transform 

```js
function a() {
  return <Button>A</Button>;
}
```

To

```js
import { Button } from 'antd-mobile';

function a() {
  return <Button>A</Button>;
}
```
## Install

```sh
npm install --save-dev babel-plugin-auto-completion
```

## Usage

### Via `.babelrc` (Recommended)

**.babelrc**

```json
{
  "plugins": ["auto-completion"]
}
```

### Via CLI

```sh
babel script.js --plugins auto-completion
```

### Via Node API

```javascript
require("babel-core").transform("code", {
  plugins: ["auto-completion"]
});
```

## Options

### `libraryName`

`string`, defaults to `""`.

xxx

### `libraryDirectory`

`string`, defaults to `"lib"`.

xxx

### `camel2DashComponentName`

`boolean`, defaults to `true`.

xxx

### `style`

`string/boolean`, defaults to `false`, `"less" "css" true"`.

xxx

### `keys`

`string/ [string]`, defaults to `[]`

xxx
