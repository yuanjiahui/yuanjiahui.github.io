title: TinyMCE基本使用
date: 2016-02-29 21:58:53
tags: TinyMCE
---
项目上需要用到文本编辑器功能，最后决定用TinyMCE插件来完成。
<!-- more -->
官网：https://www.tinymce.com

### 1. 下载文件

![cmd-markdown-logo](http://7nark3.com1.z0.glb.clouddn.com/tinymcetinymce1.jpg)
国际化文件需要单独下载 http://archive.tinymce.com/i18n/

### 2. 引入JS文件

```javascript
	<script type="text/javascript" src="js/tinymce/tinymce.min.js"></script>
```

> 引入js以后其他文件会自动引入进来不需要单独配置
![tinyMCE](http://7nark3.com1.z0.glb.clouddn.com/tinymce2.jpg)

### 3. 初始化以及参数

```javascript
	tinymce.init({
        selector: '#mytextarea', //选择器
        height: 300, //高度
        width: 600, //宽度
        statusbar: false, //底部状态栏
        language: 'zh_CN', //国际化
    });
```

### 4. 方法

```javascript
	tinymce.get("mytextarea").getContent();
```

| 方法        | 说明   								 |
| --------    | ----- 								 |
| getContent  | 获取编辑器内的HTML内容				 |
| show        | 显示所有隐藏的textarea/div编辑框   	 | 
| hide        | 隐藏所有显示的textarea/div编辑框   	 | 
| isHidden    | 判断编辑器是否隐藏 					 |


### 5. 事件

空
