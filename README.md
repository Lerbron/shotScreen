# shotScreen
# electron 的一个web截图插件工具
![示例](https://github.com/chong0808/shotScreen/blob/master/asset/images/11.png)

> 开发版本的桌面应用 https://github.com/chong0808/shotScreen/releases/tag/v1.0

### 测试案例
#### 下载之后　全局安装　electron 
#####  $ npm i electron -g

### 文件结构
```
├── dist  // 插件主要文件
│   ├── setup
│   │   ├── build  // 安装包资源
│   │   └── shotscreen-win32-x64  // 打包的文件
│   └── web // 渲染进程引入的文件
│       └── shotScreen.js //  web页面需要引入的文件
├── src  // 插件主要文件
│   ├── mainProcess
│   │   └── index.js  // 主要负责通讯
│   ├── webScripts    // web页面引用文件
│   │   └── index.js  
│   ├── index.html // 后台隐藏的常驻渲染进程
│   ├── index.js  // 接收信号
│   ├── main.js  // 应用启动文件
│   └── renderProcess // 渲染进程引入的文件
│       ├── asset  // 资源文件
│       ├── index.html // 创建截图渲染进程的文件
│       └── main.js //  创建截图渲染进程中 对图片剪切操作的文件 主要就是canvas的操作
├── README.md
└── package.json
```

### 开发模式 使用方式
```
$ npm start  // 1.启动一个测试环境web服务器 2. 启动主应用程序
```
#####　打开 http://localhost:8080/
### TODO LIST

1. 打包应用app
2. 应用自动启动
3. 应自动更新

