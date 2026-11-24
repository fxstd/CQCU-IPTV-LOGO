# CQCU-IPTV-LOGO

重庆联通 IPTV 频道台标集合。仓库根目录收录 **125 张 PNG 图片**，其中 **12 张**的文件名含有 `4K`。本仓库仅提供台标，不提供直播源或播放列表。

## 台标预览

| CCTV1 综合 | 重庆新闻 | 湖南卫视 4K | IPTV 爱电影 |
| :---: | :---: | :---: | :---: |
| <img src="./CCTV1%20%E7%BB%BC%E5%90%88.png" width="120" alt="CCTV1 综合"> | <img src="./%E9%87%8D%E5%BA%86%E6%96%B0%E9%97%BB.png" width="120" alt="重庆新闻"> | <img src="./%E6%B9%96%E5%8D%97%E5%8D%AB%E8%A7%86%204K.png" width="120" alt="湖南卫视 4K"> | <img src="./IPTV%20%E7%88%B1%E7%94%B5%E5%BD%B1.png" width="120" alt="IPTV 爱电影"> |

## 收录范围

| 频道类别 | 台标数量 | 文件示例 |
| --- | ---: | --- |
| 央视及 CGTN | 31 | `CCTV1 综合.png`、`CCTV 4K 超高清.png`、`CGTN.png` |
| 重庆本地频道 | 11 | `重庆卫视.png`、`重庆新闻.png`、`重庆红岩文化.png` |
| 其他地方卫视 | 42 | `安徽卫视.png`、`湖南卫视 4K.png`、`浙江卫视 4K.png` |
| IPTV 专题频道 | 19 | `IPTV 爱电影.png`、`IPTV 热播剧场.png`、`IPTV 少儿动画.png` |
| 中国教育电视台（CETV） | 3 | `CETV1.png`、`CETV4.png`、`CETV 早期教育.png` |
| CHC 电影频道 | 3 | `CHC 动作电影.png`、`CHC 家庭影院.png`、`CHC 影迷电影.png` |
| 其他频道 | 16 | `动漫秀场.png`、`金鹰卡通.png`、`华数TV 4K.png` |

## 在 M3U 播放列表中使用

在 M3U 播放列表的 `#EXTINF` 行中，通过 `tvg-logo` 指定台标图片地址。

```m3u
#EXTM3U
#EXTINF:-1 tvg-logo="https://raw.githubusercontent.com/fxstd/CQCU-IPTV-LOGO/main/CCTV1%20%E7%BB%BC%E5%90%88.png",CCTV1 综合
https://example.com/live/cctv1.m3u8
```

将示例中的 `https://example.com/live/cctv1.m3u8` 替换为实际播放地址。引用其他台标时，将图片地址末尾替换为对应的文件名，并对中文、空格、`+` 等字符进行 URL 编码。空格编码为 `%20`，`+` 编码为 `%2B`。
