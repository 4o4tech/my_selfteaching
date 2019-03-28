source from： [http://www.cnblogs.com/kylincat/p/9863808.html?utm\_medium=hao.caibaojian.com&utm\_source=hao.caibaojian.com](http://www.cnblogs.com/kylincat/p/9863808.html?utm_medium=hao.caibaojian.com&utm_source=hao.caibaojian.com)

**js阻止事件冒泡**

--------------

```js
　<script>

　　　　　　var div = document.getElementById("myDiv")

　　　　　　div.onclick = function(event) {

　　　　　　　　event.stopPropagation() 

　　　　　　　　// 或者直接使用return false，即阻止了事件冒泡也阻止了默认事件

　　　　　　　　// return false

　　　　　　}

 

　　</script>

```

****

**js阻止默认事件**
------------

### ** 1.通过on这种方式的绑定的事件，使用return false：**

```js
　<script>

　　　　　　var div = document.getElementById("myDiv")

　　　　　　div.onclick = function(event) { 

　　　　　　　　return false //使用return false，即阻止了事件冒泡也阻止了默认事件

　　　　　　}

　　　　</script>


```

###  2.addEventListener绑定的，使用evevt.preventDefault()：

```js


　　　　<script>

　　　　　　var div = document.getElementById("myDiv")

　　　　　　div.addEventListener( " click ",  function(event) { 

　　　　　　　　event.preventDefault()

　　　　　　})
</script>
```

**jQuery阻止事件冒泡和默认事件**
---------------------

** 阻止事件冒泡：**

** **

```js
//1.阻止默认事件：
$(document).ready(function() {
  $('#myDiv').click( function(event) {
    event.stopPropagation()
  })
})

//2.阻止默认事件：

$(document).ready(function() {
  $('#myDiv').click( function(event) {
    　event.preventDefault()
  })
})z
```

-

