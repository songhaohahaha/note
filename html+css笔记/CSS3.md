# CSS3

### 边框图片： 

先写一个边框，然后↓

引入边框图片：border-image-source：ur l（）

设置边框图片的宽度：border-image-width：48px；

切片  九个区域 fill中间区域：border-image-slice：48 fill；

定义重复： stretch 拉伸（默认值）border-image-repeat：stretch；

重复不完整 border-image-repeat：repeat；

重复完整 border-image-repeat ； round；

边框意外进行绘制的大小 外凸： border-image-outset：10px；

### 渐变

background-image：

##### 线性渐变：background-image：-webkit-linear-gradient(top/left/left top/60deg,red,yellow,pink);

(开始方向，开始颜色，结束颜色)

​	方向：top bottom left right

​	角度：0deg=left 90deg 逆时针

​	颜色可以用单词、十六进制、rgb、rgba写

不均匀的渐变：background-image：-webkit-linear-gradient(90deg,red 20%,yellow 60%,pink 70%);

重复的渐变：background-image：-webkit-repeating-linear-gradient(90deg,red,yellow 15%,pink 20%);；重复五个

##### 径向渐变：

background-image：-webkit-radial-gradient(50px 50px,red,yellow);  50px控制大小，前面加at控制位置

重复：background-image：-webkit--repeating-radial-gradient(50px 50px,red,yellow);

### 文字渐变：

先给背景渐变 background-image：-webkit-linear-gradient（）；

-webkit-text-fill-color

-webkit-background-clip：text；

### 倒影

盒子→图片→倒影 

-webkit-box-reflect：left 10px none；倒影的方向，原图和倒影的间距，遮罩效果

上above 下below 左右left 	right

遮罩效果： 1.无 none

​		    2.用url把图片引入

​		    3.渐变遮罩 方向代表原图的方向，全黑代表看的见，半透明是模糊。（不占据空间）

### 浏览器内核：

-webkit-  谷歌浏览器

-moz-     	 火狐浏览器

-ms-		 ie浏览器

-o- 		 欧朋浏览器

### 多列

column-count：4；规定列数。

column-gap：4em；规定列与列之间的间距。 em是相对于当前文本字体大小的一个单位。

column-rule：5px solid/dashed red； 列与列之间的修饰 dashed虚线

column-width：10em； 一列的最小宽度。

resize是否允许用户重新设置大小

### 外轮廓

先设置border在outline

outline:10px solid yanse;     外轮廓

outline-offset:10px;   外轮廓的相对偏移位置 ，不占空间

### 文本属性

-webkit-text-fill-color:red;   填充色

-webkit-text-stroke-width:2px;   描边粗细

-webkit-text-stroke-color:yellow;     描边颜色；

text-shadow:2px 2px 5px blue;    水平偏移量，垂直偏移量，模糊距离，阴影颜色。