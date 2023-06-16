"# h-work-2-js" 
 #  RECURSION 
  ```js
  function sum(num) {
   if (num == 0) {
      return 0
   }
   return num+ sum(num-1)
}
console.log(sum(5));
```
```js
function sum(num) {
    if (num == 0) {
        return 1
    }    
    return num* sum(num-1) 
}
console.log(sum(5));
```
```js
function sum(num) {
    if (num == 1 || num == 0) {
        return 1
    }    
    return num* sum(num-2) 
}
console.log(sum(9));
```
```js
function fibonacci(num) {
    if (num == 2 || num == 1) {
        return 1
    }
    return fibonacci(num-1)+fibonacci(num -2)

}
console.log(fibonacci(6));
```
```js
function rezult(num) {
  if (num < 10) {
    return num;
  } else {
    return num % 10 + rezult(Math.floor(num / 10));
  }
}
console.log(sumOfDigits(9999)); 
```
```js
function result(num, i = 1) {
  if (i > 10) {
    return 0;
  }
  return num * i + result(num, i + 1);
}   
const num = 1;
const sum = result(num);
console.log(sum);
```
# CLOSE
```js 
function result(a) {
    return function (b){
      if (a % b == 0) {
        return true
      }else return false
    }
  
}
const double = result(122)
console.log(double(2));
```
```js
function createMultiplier(a) {
     
    return (b)=>{
        return a*b
    }
}
let double = createMultiplier(5)
console.log(double(2));
```
```js
function rezult(a) {
     
    return (b)=>{
        return a+b
    }
}
let double = rezult(5)
console.log(double(10));
```
```js
function product(a1, b1) {
    return (a2, b2) => {
        return(a3, b3) => {
            return a1 * a2 * a3 + b1 * b2 * b3;
        }
    }
}

let double = product(1, 2)(1, 1)(2, 3);
let double2 = product(10, 2)(5, 0)(2, 3);
let double3 = product(1, 2)(2, 3)(3, 4);
console.log(double);
console.log(double2);
console.log(double3);
```
```js
function makePassword(str1) {
    return (str2) => {
        if(str1 === str2) {
            return true;
        } else {
            return false;
        }
    }
}

let sendPassword = makePassword("softclub");
console.log(sendPassword("softclub"));
```


"# h-work-2-js" 
