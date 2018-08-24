# vite-fait

```js
// (num, 5), (num, 4.5) -> (str, 'true')
Boolean(5 - 4.5).toString();
  // (num, 5), (num, 4.5)
  5 - 4.5;
  // (num, .5)
  Boolean(.5);
  // (bool, true)
  true.toString();
  // (str, 'true')

```

[replit](https://repl.it/@colevandersWands/vite-fait)

| step | state  | operation |
|---|---|---|
| 0 | (num,5), (num, 4.5) | |
| | | s0a - s0b |
| 1 | (num, .5) | | 
| | | Boolean(s1) |
| 2 | (bool, true) | | 
| | | s2.toString |
| final | (str, 'true') ||

[python tutor - trace-block](https://goo.gl/6y2DHE)

```js
function vite_fait(a, b) {
  let s1 = a - b;
  let s2 = Boolean(s1);
  let s3 = s2.toString();
  return s3;
}

vite_fait(5, 4.5);
```

[pytut - function](https://goo.gl/uQP7wa)

```js
function vite_fait(a, b, trace) {
  let result;
  if (trace) {
    result = {};
    result.args = {a, b};
  };
  
  let s1 = a - b;
  if (trace) {
    result.s1 = s1;
  };
  
  let s2 = Boolean(s1);
  if (trace) {
    result.s2 = s2;
  };
  
  let s3 = s2.toString();
  if (trace) {
    result.s3 = s3;
  };
  
  if (!trace) {
    result = s3;
  };  
  
  return result;
}

let ret_val = vite_fait(5, 4.5);
let trace = vite_fait(5, 4.5, true);

console.log(ret_val);
console.table(trace);
```

