# HTML

HTML(HyperTextMarkupLanguage 超文本标记语言) 是网页和Web应用的标准标记语言 它通过预定义的标签来结构化显示网页内容 比如 文字 图片 链接等 用不同的标签实现不同的效果 目前 最主流的HTML版本是HTML5 此文档也是HTML5的文档 写HTML Windows最推荐使用[VSCode](docs/ide/vscode) Android最推荐使用[WebCat](docs/ide/webcat)

## 结构

HTML的基础结构如下
```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8"><!--这是字符编码-->
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>我是网页标题</title>
</head>
<body>
    <p>我是段落文本</p>
</body>
</html>
```
HTML主要由头(head)和身(body)组成 head部分用来声明字符编码 写网页标题 引入外部链接(主要引入[CSS](docs/css/)和[JS](docs/js/))写样式([css](docs/css/))等 body就是写各种文字 插入图片的地方了 也可以写[JS](docs/js/)

## 标签

HTML中的所有标签都是要有闭合的 作用就是划清这个标签的开始和结束的位置 有自闭和标签:`<标签>`或者`<标签></标签>`

我们来了解一下最基本的标签
- `<!DOCTYPE>` 文档声明标签 通常在HTML文件内的第一行 写成`<!DOCTYPE html>` 我们不要管它 只需要有它就行
- `<html>` HTML文档根元素标签
```html
<!DOCTYPE html>
<html>
    你的网页内容都写在这里
</html> <!--注意最后要有闭合-->
```
- `<head>` 头标签 上面也说了 写网页标题等的地方
### `<meta>`标签
这是一个很核心但是你看不见的标签 非常重要 一般写在`<head>`标签内 用于提供HTML文档的元数据(描述数据的数据 好像有点绕喵) 浏览器或搜索引擎(例如:百度)就会通过这个来处理网页
- 字符编码:
```html
<meta charset="UTF-8">
```
这是一个必须写的标签 告诉浏览器应该用哪个编码来解析 常见的编码有"UTF-8" "GBK"等
*注意: 此标签需要写在`<head>`内第一个标签 否则浏览器可能会先解析前面的内容 导致乱码*
- 视口配置:
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<!--width=device-width: 页面宽度等于屏幕宽度-->
<!--initial-scale=1.0: 初始的缩放比例为1-->
```
这个是让页面在浏览器按照设备的宽度缩放网页
- 页面描述:
```html
<meta name="description" content="这里是网页描述">
```
网页的描述内容要写在`content=""`的双引号里面 搜索引擎会把`content=""`的双引号里面内容显示在网页标题的下面 好的描述会提高点击率 当然,如果你没让搜索引擎收录也不打算让别人发现你的网页可以不写
- 关键词:
```html
<meta name="keywords" content="这里是关键词1, 这里是关键词2, 这里是关键词3">
```
可以看到`content=""`双引号内的内容就是关键词 每个关键词中间用`,`(注意是英文输入法的逗号)分开 用于告诉搜索引擎关键词 当然,如果你没让搜索引擎收录也不打算让别人发现你的网页可以不写
- 作者或版权声明
```html
<meta name="author" content="这里是作者">
<meta name="copyright" content="这里是版权信息">
```
第一行是标注作者 第二行是标注版权信息
- 刷新或跳转
```html
<meta http-equiv="refresh" content="5">
<!--上面那里的意思是在5秒钟后刷新页面-->
<meta http-equiv="refresh" content="10; url=https://docs.nood.icu">
<!--上面那里的意思是在10秒钟后跳转至https://docs.nood.icu 也就是本文档喵~-->
```
- 兼容IE浏览器:
```html
<meta http-equiv="X-UA-Compatible" content="IE=edge">
```
让IE浏览器浏览此页面时强制使用最新渲染引擎

差不多就这些 这就是`<meta>`标签

### `<link>`标签