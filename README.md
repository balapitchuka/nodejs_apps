# Node

- NPM manages all the Node.js packages
- NPX executes the Node.js packages

# 1. Installation

## 1.Installation on linux machine

```
when we install node it shifts with node binary, npm binary and npx binary.
  url : https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-ubuntu-18-04

  installing using node version manager(NVM):
     NVM was created by the community and not the Nodejs foundation. 
    
    url : https://github.com/nvm-sh/nvm
  
```
## Useful node commands
```javascript
// check version
node -v || node --version

// list installed versions of node (via nvm)
nvm ls

// install specific version of node
nvm install 6.9.2

// set default version of node
nvm alias default 6.9.2

// switch version of node
nvm use 6.9.1
```

// update npm to latest
sudo npm install npm@latest -g

// install react cli
npm install -g create-react-app


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
module.exports = add // if you want to export only one thing also known as default export.
(or)
//exporting multiple things
module.exports = {add, value : 1, thing(){ } }    // named export


-- we have to explicitly export what ever code we will be using in other modules(public api).
-- by default nothing is exported (private ) so hence we have to explicitly export everything needed to use in other modules.

donot write module.exports to export multiple things as later statements will overide the previous module.exports.

```
