## What

项目主页面文档使用 [MkDocs](http://www.mkdocs.org/) 生成

## Prepare

* 安装MkDocs
```
    // 下载get-pip.py
    $ curl https://bootstrap.pypa.io/get-pip.py > get-pip.py
    // 安装python包管理工具pip
    $ python get-pip.py
    // 安装 mkdocs
    $ pip install mkdocs
```

* 安装gh-pages
```
    // 安装 gh-pages 工具
    $ npm install gh-pages -g
    // link gh-pages
    $ npm link gh-pages
```

* 下载项目
> 前提条件：注册 [GitHub](https://github.com) 账号后，且拥有项目 https://github.com/CardInfoLink/website 的读写权限

  ```
      $ git clone https://github.com/CardInfoLink/website
  ```

## Usage

* 修改文档  
```
    //进入项目目录
    $ cd website
    // 修改文档
    $ vi docs/index.md
    // 运行项目，预览页面
    $ mkdocs serve
    Running at: http://127.0.0.1:8000/
    // 提交修改
    $ git commit -am "此处罗列本次修改内容"
    // 推送到云端仓库
    $ git push origin master
```

* 发布页面
```
    // clean site目录
    $ mkdocs build --clean
    // build site目录
    $ mkdocs build
    // 发布页面
    $ ./publish.sh
```

## Links
* [为自己的项目生成在线文档](https://phonechan.github.io/cil-share-conference-01/)
* [markdown的基本语法](https://cardinfolink.github.io/2016/11/10/markdown-grammar/)
* [mkdocs](http://www.mkdocs.org/)
* [gh-pages](https://www.npmjs.com/package/gh-pages)
