What is a "closure"?

Closure is defined as a refernce to an instance of a local variable in a function.
Closure deals with the environment of local variables and the function.
These local variables are created every time a function is called.
It is a function inside function.The inner function has a refernce to the variables of outer function.The outer variables are
accessible to the the inner function even if the outer function is finished.

Example,

function multiply(x){
      return function(y){
          return x * y
      }
}

var multi2 = multiply(2)
var multi3 = multiply(3)


console.log(multi2(2))  // 4
console.log(multi3(4))  // 12

In example,
We have defined a function "multiply" which takes "x" as its argument and them it returns a new function.The function multiply returns 
 a code which get stored in the variable "multi2". Therfore, "multi2" becomes a function and gives output as "4".
 
 
 multi2 and multi3 are both closures but have different environments.
 In multi2, x is 2.
 In multi3, x is 3.
 
 
 
 Resources,
 https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures
 http://www.w3schools.com/js/js_function_closures.asp
 http://eloquentjavascript.net/03_functions.html
 https://ca.video.search.yahoo.com/search/video?fr=mcafee&p=videos+on+closures+of+jAVASCRIPT#id=1&vid=e546f2eafd218fafa31ba56f74565f35&action=click
 
 

