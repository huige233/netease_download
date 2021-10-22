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
