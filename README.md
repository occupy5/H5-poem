# 前言
之前看到过一个项目[Wechat-H5-Boilerplate](https://github.com/panteng/wechat-h5-boilerplate)-用于构建全屏滚动型H5页面。刚好，学校诗社举行活动需要做一个活动页面。就想着，可以用这个项目来实现。

## 预览
![h5-poem1](http://oxuk2wfkl.bkt.clouddn.com/h5_poem1.png)
![h5-poem2](http://oxuk2wfkl.bkt.clouddn.com/h5_poem2.png)

## 用到的库
1. [Animate.css](https://daneden.github.io/animate.css/)
2. [Swiper](http://idangero.us/swiper/)
3. [jQuery](https://jquery.com/)

## 目录结构 

	|-- app                            
	|-- dist                             // 打包的目录
	|   |-- audios                       // 背景音乐
	|   |-- fonts                        // ventor复制来的字体 
	|   |-- images                       // 压缩上传的图片	
	|   |-- javascript                   // js源文件
	|   |-- stylesheets                  // 由scss编译生成
	|   |-- index.html                   // 生成后的页面HTML
    |-- src                              // 项目源码
	|   |-- audios                       // 背景音乐
	|   |-- fonts                        // 字体 
	|   |-- images                       // 图片
	|   |-- javascript                   // js源文件
	|   |-- scss                         // scss文件
	|   |-- index.html                   // 整个页面的HTML文件
    |-- config                           // 项目打包路径
	|   |-- ventor.js                    // 第三方js,css列表
	|-- .gitignore                       // 忽略的文件
	|-- package.json                     // 项目及工具的依赖配置文件
	|-- gulpfile.js                      // 执行gulp任务
	|-- README.md                        // 说明

## 优化
### 响应式设计
``` css
@media all and (min-width: 400px) {    /*在屏幕宽度大于400px且小于600px的设备上，1rem = 22px*/
    html {
        font-size: 22px;
    }
}

@media all and (min-width: 600px) {   /*在屏幕宽度大于600px的设备上，1rem = 32px*/
    html {
        font-size: 32px;
    }
}
```
