## text-indent: -9999px; 只对块级元素有效(inline-block 也有效)

## overflow: hidden; 只对块级元素有效(inline-block 也有效)

## float: left; 浮动会改变元素的 display 属性，行内块，没有中间的空隙

## outline: none; input, button 的点击焦点轮廓线, outline 不可继承

## div:hover{}    hover 伪类也可以加在 div 身上

## position: absolute; 绝对定位、固定定位、浮动都会改变元素的 display 属性，行内块，没有中间空隙

## background: url() no-repeat -500px -500px; 图片会像左、上移动500px

## 垂直外边距合并 margin 塌陷; 

- 相邻垂直的两个盒子，垂直外边距合并，取外边距大的
  - 解决办法：尽量只给一个盒子添加 margin 值
- 嵌套的两个盒子，垂直外边距合并，取外边距大的
  - 解决办法：给父盒子加边框或加内边距或加个 overflow: hidden;
- 嵌套了三层盒子，给中间那层加个 display: inline-block; （float: left）也可以

## a 标签里的 color 不会继承父元素的 color, 要到 a 标签下单独设置 color 样式

## 行级元素之间的空格间隙怎么去除？

1. 给它的父元素设置 font-size: 0; 然后再给这个行级元素设置相应的 font-size
2. 让这些行级元素都浮动
3. 给它的父级元素设置 letter-spaceing: -999px; 然后再给这个行级元素设置 letter-spacing: 0;
4. 编写代码的时候去除空格

## height: 100%; 嵌套的盒子，子元素设置 height: 100%; 则 width 也相应的默认为 100% （设置 width 不行）

## 子盒子在父盒子中水平垂直居中，子盒子利用 width height 放大，也会向四周发散

## input img 等单标签不支持伪元素

## z-index 只适用于定位的元素，如 position: absolute;