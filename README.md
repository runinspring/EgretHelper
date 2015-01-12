﻿### 制作egret相关内容的小工具.基于adobe AIR。
```
请先下载运行环境:http://get.adobe.com/cn/air
```
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
### egret引擎的100多个js文件合并成一个
```
把bin-debug/lib/egret_file_list.js拖到js merge区域，其他所有工作自动完成。
使用的时候，在lancher/index.html里找到<script src="bin-debug/lib/egret_file_list.js"></script>
把egret_file_list.js后面加个2，改成egret_file_list2.js就是使用合并后的引擎。去掉2就是原来的方式。
具体的工具原理，
1.在libs下生成一个egret_all.js文件，这个就是合并后的引擎。
2.在bin-debug/lib下生成egret_file_list2.js。这个是加载单一引擎的文件
如果你不需要，可以把这2个js删掉。

```
    2015年1月12日 1.1.5 js文件合并功能改为egret专用，一键完成。
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

