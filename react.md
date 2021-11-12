# React

### 创建项目

``` javascript
npx create-react-app my-app
```

#### rewire create-react-app

##### 安装

~~~ js
npm install react-app-rewired --save-dev
~~~

##### 修改package.json运行脚本

##### 新建<code>config-overrides.js</code>文件

### 项目配置

使用<a href="https://github.com/arackaf/customize-cra">customize-cra</a>配合配置<code>config-overrides</code>文件

#### loaders

1. scss-loader (react 需要安装node-scss)

#### 工具链

##### css 作用域

##### <a href="https://www.npmjs.com/package/scoped-css-loader">scoped-css-loader</a>

##### 1.安装babel 插件

~~~ js
npm i babel-plugin-react-scoped-css -D
~~~

##### 2.配置<code>config-ovverrides</code>

~~~ js
addBabelPlugins([
      'babel-plugin-react-scoped-css',
      {
        include: '.scoped.(sa|sc|c)ss$'
      }
    ]),
~~~

##### 3.配置webpack loaders

``` js
在css-loader之前，sass-loader之后添加scoped-css-loader
```

