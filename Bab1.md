# Bab 1 Input Output Node.JS
To output something to the terminal you can use this source code
```javascript
console.log('Hello World BCC');
```

And to get input from user keyboard, it's a bit complicated. You need to use readline API from node.js
```javascript
const readline = require('readline');

const rl = readline.createInterface({
    input: process.stdin, //input from stdin
    output: process.stdout //output to stdout
});

rl.question('Input: ', (answer) => {
    console.log('Your Input: ', answer);
    rl.close();
});
```

edit kak