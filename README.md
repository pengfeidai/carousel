## 主要技术

 **v-i:** 条件渲染
 **v-for：** 列表渲染
 **v-bind：** 属性绑定
 **transition:** 过渡效果
 **组件交互:** 父组件通过 props 将数据传递给子组件

## 主要思路

轮播图中，它显示的那张图片在浏览器中可以看到有dom元素。隐藏的是没有dom元素的。所以如果显示一张图片，实际上，轮播列表中只有一个元素是存在的，其他的都被删掉了。按照这个思路，就很简单了。想要轮播，设置：enter：右边→enter-to：正常位置，并且过渡完成→leave：正常位置→leave-to：左边，并且过渡完成。

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build
