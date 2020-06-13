# 头部知识点

- header放到 container容器中去的话会自动填充整个宽度。

## 浮动问题
注意点： 当子级使用了float 时父级必须清除浮动
清除浮动的方法有三种
1、加标签
```html
<div style="clear: both;"></div>
```
2、在父级上加 overflow: hidden
```html
<header style="overflow: hidden">
```

3、最常用的,在父标签上引用下面class,class="clearfix"
```css
//清除浮动 clearfix
.clearfix:after{
    content: ".";
    display: block;
    height: 0;
    clear: both;
    visibility: hidden;
}

.clearfix{display: inline-block;}
* html .clearfix{height: 1%;}
.clearfix{display: block;}
```


## 标签

- display 可以转换标签的类型，内联或者块级元素。
```css
   img{
        display: block;//把img标签变成块级元素
    }
```
- margin 设置边距
```css
.logo{
    margin: 30px 30px 30px 30px;    //上 、右 、下 、左
    margin: 30px 30px 30px;         //上 、右左 、下 
    margin: 30px 30px;              //上下 、右左 
    margin: 30px;                   //上下右左 

    margin-top: 30px;  //上边距
    margin-bottom: 30px; //下边距
    margin-left: 30px;  //左边距
    margin-right: 30px; //右边距


}

```
























