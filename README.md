# Node

1. Installation



1.Installation on linux machine

```
  url : https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-ubuntu-18-04

  installing using node version manager(NVM):
     NVM was created by the community and not the Nodejs foundation. 
    
    url : https://github.com/nvm-sh/nvm
  
```

nodejs uses commonjs module system(by default built into nodejs).

other module systems:
commonjs - node uses by default
amd - use Requirejs
es6 modules (ESM- ecmascript script modules)

NOTE : since ECMASCRIPT introduced ESM, nodejs will eventually move to using esm module system in future.

module exporting: 
const add = (num1, num2) => {}
const nonPublic = () => {}

//module is a global object in nodejs
module.exports = add // if you want to export only one thing
(or)
//exporting multiple things
module.exports = {add, value : 1, thing(){ } }
