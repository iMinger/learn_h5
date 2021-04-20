<template>
  <div class="hello">
    <div class="container">
      <div class="col-start-end" style="height:100%">
        <div>开心吗开心吗开心吗开心吗开心吗开心吗开心吗开心吗开心吗开心吗</div>
        <div>你说呢</div>
        <div>开心</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

.flex-equally{
  flex: 1;
  text-align: center;
}

.container {
  margin: 0 auto;
  text-align: center;
  width: 300px;
  height: 300px;
  border: #42b983 2px solid;
}
/* 垂直居中，水平变化 */
/*
整体是个 row，从左到右布局
display: flex, 弹性布局，默认是从左到右布局，如果想要从上到下布局，那么就要设置flex-direction: column;
align-items: Aligns flex items along the cross axis of the current line of the flex container.
在当前弹性盒子容器的副轴方向上对子元素进行弹性排布，center:居中排布
justify-content: 
Aligns flex items along the main axis of the current line of the flex container.
在当前弹性盒子容器的主轴方向上对齐子元素
*/
.row-center-start {
  display: flex;
  align-items: center;
  justify-content: flex-start;
}

.row-center-center {
  display: flex;
  align-items: center;
  justify-content: center;
}

.row-center-end {
  display: flex;
  align-items: center;
  justify-content: flex-end;
}

/* around: prep 四处，在。。。周围 。
justify-content: space-around; 表示每个元素周围都有空间，最左右两遍也有空间
 */
.row-center-around {
  display: flex;
  align-items: center;
  justify-content: space-around;
}

/* space-between 空间均分,最左右靠边 */
.row-center-between {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

/* 垂直居上，水平变化 */
.row-start-start {
  display: flex;
  align-items: flex-start;
  justify-content: flex-start;
}
.row-start-center {
  display: flex;
  align-items: flex-start;
  justify-content: center;
}

.row-start-end {
  display: flex;
  align-items: flex-start;
  justify-content: flex-end;
}

.row-start-around {
  display: flex;
  align-items: flex-start;
  justify-content: space-around;
}

.row-start-between {
  display: flex;
  align-items: flex-start;
  justify-content: space-between;
}

/* evenly 和 around 的区别是： 
around 最两端两边的空白是中间空白的一半
而evenly 两边留的空白跟中间留的空白是一样大的 */
.row-start-evenly {
  display: flex;
  align-items: flex-start;
  justify-content: space-evenly;
}

/* 垂直居下， 水平变化 */

.row-end-start {
  display: flex;
  align-items: flex-end;
  justify-content:  flex-start;
}

.row-end-center {
  display: flex;
  align-items: flex-end;
  justify-content: center;
}

.row-end-end {
  display: flex;
  align-items: flex-end;
  justify-content: flex-end;
}

.row-end-around {
  display: flex;
  align-items: flex-end;
  justify-content: space-around;
}

.row-end-between {
  display: flex;
  align-items: flex-end;
  justify-content: space-between;
}

.row-end-evenly {
  display: flex;
  align-items: flex-end;
  justify-content: space-evenly;
}


/* 水平居中，垂直变化 
整体是个 column ，竖直方向上依次排布。因为 display:flex 默认是水平方向排布的，
也就是说 flex默认是 row 排布，所以如果想让 flex 是竖直方向上排布，需要设置一下排布方向：
flex-direction: column.

*/
.col-center-start {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: flex-start;
}

.col-center-center {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.col-center-end {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: flex-end;
}

.col-start-start {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: flex-start;
}

.col-start-center {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: center;
}

.col-start-end {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: flex-end;
}



</style>
