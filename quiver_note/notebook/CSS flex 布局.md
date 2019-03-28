<http://www.ruanyifeng.com/blog/2015/07/flex-examples.html>

Flex 的 六个属性

* flex-direction // `flex-direction`属性决定主轴的方向（即项目的排列方向）。
* flex-wrap
* flex-flow
* justify-content
* align-items
* align-content

```css

.box {
  flex-direction: row | row-reverse | column | column-reverse;
}

```

* `flex-direction`

-----------------------

  * `row`（默认值）：主轴为水平方向，起点在左端。
  * `row-reverse`：主轴为水平方向，起点在右端。
  * `column`：主轴为垂直方向，起点在上沿。
  * `column-reverse`：主轴为垂直方向，起点在下沿。



```html
<div class="box">
  <span class="item"></span>
</div>


<style>
  .box{
    display:flex;
  }
  
  .box{
    display: flex;
    justify-content: center; // 居中
  }
</style>
```

设置项目的对齐方式，就能实现居中对齐和右对齐。

```
justify-content
```

