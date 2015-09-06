iconfont平台字体图标
=====
详细参考 [foo]: http://iconfont.cn  "Optional 


## 第一步：使用font-face声明字体
####引入ttf、eot、svg、woff等文件详细参考 [foo]: http://iconfont.cn/help/platform.html  "Optional Title Here"

```shell
@font-face {font-family: 'iconfont';
    src: url('iconfont.eot'); /* IE9*/
    src: url('iconfont.eot?#iefix') format('embedded-opentype'), /* IE6-IE8 */
    url('iconfont.woff') format('woff'), /* chrome、firefox */
    url('iconfont.ttf') format('truetype'), /* chrome、firefox、opera、Safari, Android, iOS 4.2+*/
    url('iconfont.svg#iconfont') format('svg'); /* iOS 4.1- */
}
```

## 第二步：定义使用iconfont的样式

```shell
.iconfont{
    font-family:"iconfont" !important;
    font-size:16px;font-style:normal;
    -webkit-font-smoothing: antialiased;
    -webkit-text-stroke-width: 0.2px;
    -moz-osx-font-smoothing: grayscale;}
```


## 第三步：挑选相应图标并获取字体编码，应用于页面
```
# 第一种方法：编码写到文本块里
<i class="iconfont">&#x33;</i>

＃第二种方法：编码用伪类选择器的方式
.icon:before { content: "&#x33"; }
<i class="iconfont icon"></i>
```