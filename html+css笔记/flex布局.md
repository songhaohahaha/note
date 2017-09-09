# flex布局 弹性布局

display:flex;给容器加

设置为弹性盒模型   里面的每个子元素叫项目，当设置为弹性盒模型之后，子元素float  clear vertical-align失效。

在容器中水平方向的叫主轴，垂直方向叫做交叉轴。互相垂直。

justify-content:space-between;  

justify-content:space-around;

padding设置上下左右距离。

##### 阮一峰。

### 容器属性

1.主轴的方向：	   row：主轴方向在水平方向，项目排布从左向右。

​				   flex-direction：row-reverse;主轴方向还是水平方向，项目排布从右向左；

​				   flex-direction:column;主轴方向在垂直方向，项目排布从上到下。

​			      	   flex-direction:column-reverse;主轴方向在垂直方向，项目排布从下到上。

2.项目换行

​				flex-wrap:   nowrap;不换行

​				flex-wrap：wrap； 换行

​				flex-wrap：wrap-reverse；换行，项目从下往上。

3.项目在主轴方向的对齐方式：

​				justify-content：flex-start；主轴的起点。

​				justify-content：flex-end；主轴的终点。

​				justify-content：center；主轴的中点

​				justify-content：space-between；项目的两端对齐，剩余空间平均分布。

​				justify-content：space-around； 每个项目两端的距离相同，中间距离是两边距离的二倍。

4.项目在交叉轴方向的对齐方式align-items

​				align-items:flex-start;  交叉轴的起点

​				align-items:flex-end;交叉轴的终点

​				align-items:center;交叉轴的中点

​				align-items:baseline；基于基线（文本的底部）进行对齐；

5.基于多轴，项目在交叉轴方向的对齐方式

​				align-content:flex-start；交叉轴的起点。

​				align-content:flex-end；交叉轴终点。

​				align-content:center；交叉轴的中点

​				align-content:space-between；项目的两端对齐，剩余空间平均分布。

​				align-content:space-around； 每个项目两端的距离相同，中间距离是两边距离的二倍。

### 项目属性order

1.项目的排列顺序 order （加在子元素身上）

​	数值越小越靠前，默认值是0，可以识别负数。

2.项目的放大比例，默认值为0（即使存在剩余空间也不进行放大）

flex-grow 所有项目放大比例为1时，对剩余空间等分

​		 属性为2的时候，设置为2的，分的时候占两份；

  3.项目的缩小比例flex-shrink默认值为1，空间不足，进行缩小。值设置为0的话，即使空间不足，也不进行缩小。

4.项目占据主轴空间的值，flex-basis；

5.align-self  给单独项目定义交叉轴上的对齐方式。

