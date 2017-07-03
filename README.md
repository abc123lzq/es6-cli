### 这是一个学习es6运行框架

> 由于搭建环境比较中高级所有新手可以不用自己搭建直接引用就行

第一： 安装package.json依赖
```
cnpm install

```
第二： 安装express服务器

> 在server文件夹里安装

```
express --ejs

cnpm install
```
第三：在server里的app.js 加入热更新

```
app.use(express.static(path.join(__dirname, 'public')));
app.use(require('connect-livereload')());

```
第四： 根目录下运行gulp

```
gulp --watch

//游览器输入  http://localhost:3000/

```

第五： 查看时候运行成功

> 在app里的views里的index.ejs里谁便书写内容保存看游览器能热更新就可以了
