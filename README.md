# 91porn_share
91porn api免费分享

# API版接口 

接口: https://api.zhaiclub.com/source/

## 接口：获取视频列表
| 描述     | 内容               |
| -------- | ------------------ |
| 接口功能 | 请求91porn视频资源 |
| 请求协议 | HTTPS              |
| 请求方法 | GET                |
| 请求url  | source_list           |
| 响应格式 | json               |

### 请求参数

| 参数     | 描述                                             | 必填 | 类型   |
| -------- | ------------------------------------------------ | ---- | ------ |
| viewkey  | 视频播放id                                             | 否  | string    |
| page     | 页码                                             | 否  | int    |
| title     | 标题                                           | 否  | string   |
| author     | 作者                                             | 否  |  string   |
| up_time     |上传时间                                             | 否  | string   |
| is_91_del     | 是否已被91删除                                        | 否  | int    |



### 响应参数

| 参数        | 描述                     | 必有 | 类型          |
| ----------- | ------------------------ | ---- | ------------- |
| status   | 状态码                   | 是   | String        |
| msg | 状态消息                   | 是   | String        |
| count| 总数         | 是   | String        |
| data | 视频列表，object格式见下 | 是   | Array[Object] |


list object结构,如下：

| 参数       | 描述        | 必有 | 类型   |
| ---------- | ----------- | ---- | ------ |
| viewkey    | 视频viewkey | 是   | String |
| img      | 视频图片    | 是   | String |
| author        | 作者 | 是   | String |
| up_time   | 上传时间    | 是   | String |
| title   | 视频标题    | 否   | String |
| vid | 视频id    | 是   | String |
| duration | 视频长度  | 是   | String |
| video_url | 视频地址  | 是   | String |
| is_91_del | 91是否删除  | 是   | String |

### 请求示例

```
https://api.zhaiclub.com/source/source_list?title=电话
```

### 响应示例


```
{
    "status": "200",
    "msg": "返回成功",
    "data": {
        "list": [
            {
                "viewkey": "059b36612c5ab4adb070",
                "image": "https://img.t6k.co/thumb/386264.jpg",
                "author": "Zyusn99_  ",
                "up_time": "2020-07-30",
                "title": "操着接老公电话，差点被听出来，对话刺激，已婚少妇的快乐！",
                "vid": "386264",
                "duration": "09:16",
                "video_url": "https://down.zhaiclub.com/videos.php?vid=386264",
                "is_91_del": 0
            }
}
```

###服务器成本比较高，有钱捧个钱场
BTC 1CuUZZEDhG4SzcwHu9GgaTGm1bbvX2e4cp

