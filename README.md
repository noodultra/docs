# 喵~
*最后编辑于2026/06/09 by:nood*

## 提示
此文档是给开发的小南梁阅读的 如果你要查看我们写好的文档 请前往我们的[网站](https://docs.nood.icu)

## 开源声明

此项目使用MIT开源协议 版权归面缶所有 © 2026 面缶.All rights reserved.

## 文件路径

```text
project/
├── docs/ #工作目录
│   ├── .vitepress #VitePress专用配置目录
│   │    ├── cache #缓存目录
│   │    ├── dist #构建产物目录
│   │    │    └── ... #构建后的产物文件
│   │    ├── theme #主题目录
│   │    │    ├── index.js #主题入口文件
│   │    │    └── custom.css #自定义样式文件
│   ├── docs #文档目录 全是大家共同编写的文档呢喵
│   │    ├── index.md #索引 也就是网站中常见的index.html
│   │    └── ... #其他md文档
│   ├── public #静态资源目录
│   │    ├── images #图片存放目录
│   │    │    └── ... #各种图片
├── node_modules/ #node依赖包
│    └── ... #依赖文件
├── package.json #项目配置文件
├── package-lock.json #npm生成文件
├── CHANGELOG.md #更新日志
└── README.md #帮助文件 也就是此文件喵
```
各位小南梁 上方就是项目的文件路径表 一般要写文档的话 访问./docs/docs 就可以了 听话点 好好写啊喵

## 文档格式

- 标题用"#"开头 写标题 比如: `# 这是一个标题`
- 再往下就写最后的编辑日期和作者 比如: `*最后编辑于2026/06/09 by:nood*`
- 再往下就写本文档的介绍 开头必须是: `欢迎来到小南梁的编程手册 xxx第x节`
- 下面每一个部分就写"##"加标题就行了 比如: `## Python3介绍`
- 最后加个结束语就完了

如果你觉得自己写的不好也可以试试ai呢喵

## 在本地查看

*适用于Windows*

打开cmd 在终端输入
```bash
node -v
npm -v
```
确保你已经安装了node.js和npm

cmd cd进入项目文件夹 然后输入:
```bash
npm run docs:dev
```
启动本地服务器 然后打开浏览器输入`http://localhost:5173/`或者点击[此处](http://localhost:5173/)去网页

## 构建

*适用于Windows*

打开cmd 在终端输入
```bash
node -v
npm -v
```
确保你已经安装了node.js和npm

cmd cd进入项目文件夹 然后输入:
```bash
npm run docs:build
```
完成构建 构建后的产物在`.\docs\.vitepress\dist`

## 鸣谢

感谢各位小南梁的付出 为《小南梁的编程手册》添砖加瓦呢喵!

### 贡献者列表

- 面缶

© 2026 面缶.All rights reserved.