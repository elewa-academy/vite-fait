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

[python tutor](https://goo.gl/6y2DHE)
