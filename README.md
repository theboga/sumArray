# Sum an array values JavaScript
To Sum an Array values Javascript is very easy

## `The Fast Method`


using reducer 
[array].reduce((accumulator, currentValue) => accumulator + currentValue, defaultValue)
~~~ javascript
const sumTotal = [1,2,3,4].reduce((a, b) => a+b, 0) // return 10
~~~
## Example:

~~~ javascript
console.log(
  [1, 2, 3, 4].reduce((a, b) => a + b, 0)
) // return 10


console.log(
  [].reduce((a, b) => a + b, 0)
)
~~~

Let's do it you have an array like this:
~~~ javascript
const arr = [1, 2, 3, 4];
~~~
To sum all values show some algoritms:

### 1) Using built-in reduce()

~~~ javascript
function total(arr) {
  if(!Array.isArray(arr)) return;
  return arr.reduce((a, v)=>a + v);
}
~~~
### 2) Using the command's for loop

~~~ javascript
function total(arr) {
  if(!Array.isArray(arr)) return;
  let totalSum = 0;
  for (let i=0,l=arr.length; i<l; i++) {
     totalSum+=arr[i];
  }
  return totalSum;
}
~~~

### 3) Using comand's while loop

~~~ javascript
function total(arr) {
  if(!Array.isArray(arr)) return;
  let totalSum = 0, i=-1;
  while (++i < arr.length) {
     totalSum+=arr[i];
  }
  return totalSum;
}

~~~
### 4) Using array forEach

~~~ javascript
function total(arr) {
  if(!Array.isArray(arr)) return;
  let totalSum=0;
  arr.forEach(each => {
    totalSum+=each;
  });
  return totalSum;
};
~~~
### Call to the function:

~~~ javascript
total(arr); //return 10
~~~ 
