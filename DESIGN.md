# Tutorial-typescript-package
How to implement a nodejs app using Typescript

# Inspiration 
Flexibility is great because it allows to get something done quickly, but this leaves a big room for errors/bugs/instability.
In Javascript world, this Flexibility is the ability to
* Assign values of different types to the same variable
* 

Typescript not only reduces this room of instability, but also provides a clean way to write organized code.

Example
```javascript

```

```typescript

```

# We are building
A task runner that periodically execute a given javascript function. We call this `perpetual`.

# Usage and Thinking
There is a default runner that only executes a "one" javascript function given as input
```
const perpetual = require('perpetual');
const runner = perpetual.defaultRunner();
runner.setDelay();
let task = function(input) { console.log('input is' + input); };
let args = [100];
runner.addTask(task, args);
runner.start();
runner.stop();
```
Behind the scene, starting a task is the same as running the function in this form `(function(input){ console.log('input is' + input); })(100);`.

# Steps
* Download typescript
* Download gulp
* Project setup 
```
root
  - compiled // javascript code ( translated from typescript )
  - src // writen typescript code
  - package.json
  - gulpfile.js
```
* 




