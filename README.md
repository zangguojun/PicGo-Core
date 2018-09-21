## PicGo - Core

![standard](https://img.shields.io/badge/code%20style-standard-green.svg?style=flat-square)
![GitHub](https://img.shields.io/github/license/mashape/apistatus.svg?style=flat-square)
![Travis (.org)](https://img.shields.io/travis/PicGo/PicGo-Core.svg?style=flat-square)
![npm](https://img.shields.io/npm/v/picgo.svg?style=flat-square)

![](https://raw.githubusercontent.com/Molunerfinn/test/master/picgo/picgo-core-fix.jpg)

A tool for picture uploading. Both CLI & api supports.


## Installation

### Global install

```bash
npm install picgo -g

# or

yarn global add picgo
```

### Local install

```bash
npm install picgo -D

# or

yarn add picgo -D
```

## Usage

### Use in CLI

> PicGo uses `SM.MS` as the default upload pic-bed.

Show help:

```bash
$ picgo -h

  Usage: picgo [options] [command]

  Options:

    -v, --version                 output the version number
    -d, --debug                   debug mode
    -s, --silent                  silent mode
    -c, --config <path>           set config path
    -h, --help                    output usage information

  Commands:

    install|add <plugins...>      install picgo plugin
    uninstall|rm <plugins...>     uninstall picgo plugin
    update <plugins...>           update picgo plugin
    set|config <module> [name]    configure config of picgo modules
    upload|u <input...>           upload, go go go
    choose|ch [options] [module]  choose modules of picgo
```

#### Upload a picture from path

```bash
picgo upload /xxx/xx/xx.jpg
```

### Use in node project

```js
const PicGo = require('picgo')
const picgo = new PicGo()

picgo.upload(['/xxx/xxx.jpg'])
```

## Documentation

For more details, you can checkout [documentation](https://picgo.github.io/PicGo-Core-Doc/).