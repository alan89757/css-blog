## CSS 盒子模型（Box Model）

#### 先看一张盒子模型图

<img src="./images/box-model.gif">

**说明：**
- Margin, 外边距，外边距是透明的
- Border, 围绕着内边距和内容的边框
- Padding, 内边距，内边距是透明的
- Content, 盒子内容，显示文本，css设置元素宽度和高度，就是在设置Content

####  计算总元素占据空间大小

看如下示例代码：
```js
div#box {
    width: 300px;
    border: 10px solid green;
    padding: 20px;
    margin: 30px;
}
```

div元素占据空间大小（420px）：`300px（宽度） +  40px(左+右填充) + 20px(左+右边框) + 60px(左+右外边距)`

##### 总结：
总元素宽度=宽度+左填充+右填充+左边框+右边框+左边距+右边距
总元素高度=高度+顶部填充+底部填充+上边框+下边框+上边距+下边距


