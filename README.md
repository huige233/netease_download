## 名字(Name)

netease_download -- 一款简单且极少依赖的网易云音乐下载器，支持根据网易歌曲详情修改mp3的id3 tag信息

## 使用(Useage)

需要python3

**注意：**
1. 如果是windows的cmd/powershell,默认字符集是GBK，部分歌名会报错，所以需要运行 `CHCP 65001`。
2. 部分歌曲下架后，下载时会提示，暂无版权。


```cmd
cd netease_download
pip install -r requestments.txt

python main.py http://music.163.com/#/song?id=27836179 # 单曲
python main.py http://music.163.com/#/album?id=37253721 # 专辑
python main.py http://music.163.com/#/playlist?id=2225407480 # 歌单
python main.py http://music.163.com/#/discover/toplist?id=1978921795 # 流行榜
python main.py http://music.163.com/#/artist?id=905705 # 艺术家
python main.py http://music.163.com/#/djradio?id=526696677 # 电台节目
python main.py http://music.163.com/#/program?id=1369232209 # dj
```
### 有关 现有版本

本工具目前因为网易云的网页端调用修改

只能使用单曲和歌单内容 歌单一次只能拉取10首

电台单曲也可以使用 但是文本存在一定错误

## 鸣谢(Thanks)

本工具借鉴了下面三个优秀开源项目的代码，特此注明

- https://github.com/Jack-Cherish/python-spider.git  (Encrypyed 部分)

- https://github.com/PeterDing/iScript.git (50%+的代码,包括但不限于根据url解析不同分属，修改id3 tag,解析歌曲信息,但是下载部分改用py原生，大部分接口改用网易api)

- https://github.com/Binaryify/NeteaseCloudMusicApi.git (api的uri和参数调用部分)

## 反馈(Feedback)

如果有问题，欢迎提 [issues][]

Copyright and License
=====================

This module is licensed under the BSD license.

Copyright (C) 2018-, by huige233 <huige1463@gmail.com>.

All rights reserved.

Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:

* Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.

* Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

