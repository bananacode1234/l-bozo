# l-bozo
get the raw l bozo string by running this (non async): 
```js
fetch("https://raw.githubusercontent.com/bananacode1234/l-bozo/main/l-bozo.txt").then(x=>{x.text().then(x=>{window.lbozo=x.replace("\n","")})});
```

async version: 
```js
window.lbozo=(await(await fetch("https://raw.githubusercontent.com/bananacode1234/l-bozo/main/l-bozo.txt")).text()).replace("\n","");
```

call the lbozo string with `lbozo`

example: `console.log(lbozo);`
