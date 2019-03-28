```js
(参数1, 参数2, …, 参数N) => { 函数声明 }
(参数1, 参数2, …, 参数N) => 表达式（单一）
//相当于：(参数1, 参数2, …, 参数N) =>{ return 表达式; }

// 当只有一个参数时，圆括号是可选的：
(单一参数) => {函数声明}
单一参数 => {函数声明}

// 没有参数的函数应该写成一对圆括号。
() => {函数声明}




-- ////////////////////////////

x => x * x

//等于 

function (x) {
    return x * x;
}
```

promise 没有返回值 直接调用方法使用

```js

function fn1() {
    return new Promise(function(resolve, reject) {
        // ... some code

        if ( /*异步操作成功*/ ) {
            resolve(value)
        } else {
            reject(error);
        }
    });s
}


//
fn1().then(value => console.log(value))

//
fn1().then(function(value){
    //do something
})


```

