Wolfram - a Wolfram|Alpha API wrapper for Node.js
=================================================

Wolfram is a simple Wolfram|Alpha API wrapper for Node.js.
Currently it supports only answers with primary results with plaintext answers but pod image support will be added in the future.

How to use
----------

Register for an application ID in the [Wolfram|Alpha developer website](http://products.wolframalpha.com/developers/). 

Install the module with npm:
`$ npm install wolfram`

Example usage:

```javascript
var wolfram = require('wolfram').createClient("[CENSORED]")

wolfram.query("integrate 2x", function(err, result) {
  if(err) throw err
  console.error("result", result)
})
```

License
-------

MIT