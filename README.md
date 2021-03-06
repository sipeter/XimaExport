# XimaExport--为喜马拉雅app导出的音频文件自动重命名

## 功能说明：

喜马拉雅是一个流行的音频、音乐分享平台。用户可以在有无线网络链接时下载音频之后离线收听。但是大量的音频下载会占据手机存储空间。若想将手机中下载的音频导出到电脑上，用户可以依据各自的手机系统（苹果或安卓或其他，详见下文）将相关文件拷贝到电脑上。但是这样获得的音频文件均没有可识别的文件名（如0f25cbfa4d1c017ec568769d9eef66cf），也没有专辑分类。

XimaExport 可以帮助你批量重命名音频文件，按专辑分类存储，并下载专辑封面，完善音频文件元数据。

## 安装：

1. 免安装可执行程序：
  * win10 用户：到Onedrive (https://1drv.ms/u/s!ADPhQHKDm7rqgQw) 或者 dropbox (https://dl.dropboxusercontent.com/u/74222489/ximaexport-gui.rar) 或者某度云盘 (https://pan.baidu.com/s/1pL5vbzP) 下载ximaexport-gui.rar。解压。
  * win7 用户：暂无
  * Mac 用户：暂无


2. 执行python代码：
  确保以下 dependencies 满足：
  * pandas
  * sqlite3
  * mutagen (可选）
  
  下载代码后，运行
  `python ximaexport-gui.py`


## 使用

1. 获得喜马拉雅数据文件：
  
  （1）苹果用户：链接电脑itunes，在app一栏中找到“喜马拉雅”，单击，右侧会出现“喜马拉雅”的数据文件。选择“iDoc”，并导出到电脑。

  （2）安卓用户：链接电脑后，拷贝出ting文件夹。
  
  （3）其他系统：不详。欢迎用户提供信息。

2. 运行ximaexport-gui。

    1. 在 “ting.sqlite文件”一栏，选择步骤1中拷贝出的文件夹里的 ting.sqlite 文件。
    2. 在 “导出到文件夹”一栏，选择音频存储位置。
    3. 在 “专辑”下拉菜单，选择要导出的专辑。若全部导出选择“All”。
    4. 点击“开始”开始处理。

## 已知问题

* 拷贝出的文件添加 .mp4 后缀，主要是因为喜马拉雅下载的音频文件确实是以 mp4 格式 （aac he-aacv2）格式存储的。如果改为 .mp3 后缀，仍然可以用播放器打开，但是将无法导入到 itunes。

## Licence

Copyright 2016 Guang-zhi XU

This file is distributed under the terms of the GPLv3 licence. See the LICENSE file for details.
You may use, distribute and modify this code under the terms of the GPLv3 license.




