[![Codacy Badge](https://api.codacy.com/project/badge/grade/874e7dce623149e18807bdc0a02671c2)](https://www.codacy.com/app/se-panfilov/mini-toastr)
[![bitHound Overall Score](https://www.bithound.io/github/se-panfilov/mini-toastr/badges/score.svg)](https://www.bithound.io/github/se-panfilov/mini-toastr) [![bitHound Code](https://www.bithound.io/github/se-panfilov/mini-toastr/badges/code.svg)](https://www.bithound.io/github/se-panfilov/mini-toastr)
[![Code Climate](https://codeclimate.com/github/se-panfilov/mini-toastr/badges/gpa.svg)](https://codeclimate.com/github/se-panfilov/mini-toastr)
[![Build Status](https://travis-ci.org/se-panfilov/mini-toastr.svg?branch=master)](https://travis-ci.org/se-panfilov/mini-toastr)
[![devDependency Status](https://david-dm.org/se-panfilov/mini-toastr/dev-status.svg)](https://david-dm.org/se-panfilov/mini-toastr#info=devDependencies)
[![GitHub license](https://img.shields.io/github/license/mashape/apistatus.svg)](https://github.com/se-panfilov/mini-toastr/blob/master/LICENSE)

[![NPM](https://nodei.co/npm/mini-toastr.png?downloads=true&downloadRank=true&stars=true)](https://nodei.co/npm/mini-toastr/)

# mini-toastr

**mini-toastr** - it's a small non-blocking notification library. No dependencies.

================

##Instalation

1. Install

via npm:

```shell
npm i mini-toastr --save
```

via bower:

```shell
bower i mini-toastr --save
```
or download [latest release][1]

2. Include in project

include in project:

```HTML
<script src="bower_components/mini-toastr/mini-toastr.js"></script>
```

or

```JS
import miniToastr from 'mini-toastr' //ES6
```

```JS
Vue.use(VueNotifications, options)
```

3. Init

```JS
miniToastr.init()// config can be passed here miniToastr.init(config)
```

##Usage

```JS
miniToastr.success(message, title, timeout, cb, config)
miniToastr.info(message, title, timeout, cb, config)
miniToastr.warn(message, title, timeout, cb, config)
miniToastr.error(message, title, timeout, cb, config)
```

*Attention:* You can specify your own types in global config: `miniToastr.init({types: debug: 'debug'})` and use it - `miniToastr.debug(message, title, timeout, cb, config)`

##Methods arguments

| Name | Type | Default | Required | Description | 
|---|---|---|---|---|
| `message` | `String` | `undefined` | Yes | Message in notification |
| `title` | `String` | `undefined` | No | Title for notification |
| `timeout` | `Number` | `3000` | No | Time before notification gone |
| `cb` | `Function` | `undefined` | No | Callback function |
| `config` | `Object` | `undefined` | No | Local config for this menthod call |

##License

MIT License

Copyright (c) 2016 Sergey Panfilov

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.


[1]: https://github.com/se-panfilov/mini-toastr/releases
