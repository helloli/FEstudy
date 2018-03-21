[TOC]

## 外边距合并

块级元素的 `margin-top` 和 `margin-bottom` 属性有时候会被合并(折叠)成单个边距，折叠后的值是两者中最大的那个，这种行为被称为 **外边距塌陷** 或者 **外边距合并(margin collapsing)**。

本文讨论发生外边距合并的三种常见情况，发生外边距合并时外边距的计算方法，以及避免发生外边距合并的几种解决方案。

### 一、 发生外边距合并的三种情况

**相邻的兄弟元素**

相邻的两个兄弟元素之间的外边距会塌陷。如：

```
<p style="margin-bottom: 30px;">这个段落的下外边距被合并...</p>
<p style="margin-top: 20px;">...这个段落的上外边距被合并。</p>
```

两个 p 标签的实际外边距是30px，即两个 margin 中的较大者。

**块级父元素与其第一/最后一个子元素**
**相邻的兄弟元素**

### 二、 发生外边距合并时外边距的计算方法

### 三、 避免发生外边距合并的几种解决方案

### 参考文档：

1. [https://developer.mozilla.org/en/docs/Web/CSS/CSS_Box_Model/Mastering_margin_collapsing](https://developer.mozilla.org/en/docs/Web/CSS/CSS_Box_Model/Mastering_margin_collapsing)
2. [http://www.w3help.org/zh-cn/kb/006/](http://www.w3help.org/zh-cn/kb/006/)
3. [http://stackoverflow.com/questions/35257018/how-to-disable-margin-collapse-between-sibling-elements](http://stackoverflow.com/questions/35257018/how-to-disable-margin-collapse-between-sibling-elements)