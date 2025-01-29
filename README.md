# Mystery Function

What does the `mystery()` function in the following piece of code do? Add your
answer to this markdown file.

This function first checks if there is only one element in an array, if there is only one element it returns that element. If there are more than one element it then takes off an element and assigns it to foo. If foo is more than the first element in the array it returns foo to the function again using recursion and checks the first condition again, if foo is less than the first element, it will return the first element in the array. Given an array, this function will return the greatest element in the array.

```javascript
function mystery(a) {
    if(a.length == 1) return a[0];
    var foo = mystery(a.slice(1, a.length))
    if(foo > a[0]) return foo;
    else return a[0];
}
```
I submitted this work Fall 2024.

I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.
