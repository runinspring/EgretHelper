﻿制作egret相关内容的小工具.基于adobe AIR。
请先下载运行环境:http://get.adobe.com/cn/air
------
### base64 图片
```
egret启动的时候可以先显示一个logo，是base64的字符串
把png图片拖拽进指示框内，就会在桌面生成一个对应的txt文件。
```
### 生成二维码图片
```
输入链接地址，点击保存按钮，会在桌面上生成 QRCode.png
支持把自定义的图片拖拽到二维码中间。中间的大小为50x50，请先处理好图片。
```
### 多个js文件合并成一个
```
参考JSMergeExample文件夹
里面有一个file_list.js文件(文件名不限，后缀不限，文本格式就可以)。
这里面是需要合并的js文件列表，用逗号隔开。加载路径是相对路径。
把file_list.js拖到js merge区域，就会在桌面上生成一个egretjs.js文件。
这个js文件就是文件列表里的内容打包到一起后生成的。
对于egret来说，把bin-debug/lib/egret_file_list.js 拷贝到libs文件夹里，
然后拖拽到js Merge里就行了。
```
    2015年1月1日 1.1.4 增加egret默认的egret_file_list.js文件列表直接读取功能
    2014年12月26日 1.1.3 增加多个js文件合并成一个js文件的功能
    2014年10月06日 1.1.2 去掉二维码默认的http开头
    2014年9月11日 1.1.1 修改错误拼写的说明文字
    2014年9月 7日 1.1.0 重新绘制了界面，成为一个正式软件。优化逻辑代码。
    2014年9月 1日 1.0.9 取消二维码中间的默认logo
    2014年8月29日 1.0.8 移除删减类的功能，添加生成二维码的功能
    2014年8月12日 1.0.7 增加base64 jpg格式的支持，限制图片的最大体积为50k
    2014年8月11日 1.0.6 解决mac系统下的一个兼容问题
    2014年8月11日 1.0.5 增加base64的png图片生成功能

