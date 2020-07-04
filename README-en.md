## Babel Js Environment Example

This repository aims to provide a JavaScript development environment capable of using the latest features while still being compatible with older browsers
### Prerequisites

- Node
- NPM
- Git

### Instalação


First clone this repository in the location you find most appropriate using the following command:
```bash
git clone https://github.com/lynconEBB/babelJS-example.git
``` 

After that install the dependencies used with the following command:
```bash
npm install --dev
```

### Usage

This structure was created to be as simple as possible to use, just put your codes in the [src](https://github.com/lynconEBB/babelJS-example/tree/master/src) folder  and the converted code will be included in the [out](https://github.com/lynconEBB/babelJS-example/tree/master/out) folder.
 
If you want to transform your codes just once, use the command:
```bash
npm run build 
```

Or if you want to write your codes and automatically convert them every time you save, use the command:
```bash
npm run watch
```

### Configuração

Any changes to the Babel settings can be made in the [babel.config.json](https://github.com/lynconEBB/babelJS-example/blob/master/babel.config.json) file.

To change the browsers that you want to guarantee compatibility, just change the _targets_ parameter. This parameter can be a JSON object containing the name of the browsers and their versions or a query in the [browserslist format](https://github.com/browserslist/browserslist#queries).
```JSON
{
"presets": 
[
  [
    "@babel/env",{
      "targets": {
        "chrome": "58",
        "ie": "11"  
      }  
    }
  ]
 ]
}
```