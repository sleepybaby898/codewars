# 6kyu - javascript

## Take a Ten Minute Walk
https://www.codewars.com/kata/take-a-ten-minute-walk/train/javascript

```javascript
function isValidWalk(walk) {
  var directions = {
    n: 0,
    e: 0,
    s: 0,
    w: 0
  };
  walk.forEach((element) => (directions[element] += 1));
  
  if(walk.length == 10 && directions.n == directions.s && directions.e == directions.w) {
    return true
  } else {
    return false
  }
}
```
