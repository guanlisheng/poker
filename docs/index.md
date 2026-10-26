---
layout: page
title: "Poker MTT · 赛事终端"
---

一块屏幕管住整场比赛。盲注时钟、终端配对、多屏同步、语音播报，一次配置，全场同步。

下面 12 个篇幅从"你会在电视上看到什么"出发，逐个介绍这套系统怎么用、适合什么规模的俱乐部、第一次上手能免费体验到什么程度。

## 先看整体演示

<div style="position:relative;width:100%;padding-bottom:56.25%;margin:1.5rem 0;overflow:hidden;border-radius:8px;background:#0d1117;">
  <video
    controls
    playsinline
    preload="none"
    poster="./media/poker-introduction-poster.jpg"
    style="position:absolute;inset:0;width:100%;height:100%;object-fit:cover;background:#000;">
    <source src="./media/poker-introduction.mp4" type="video/mp4">
    你的浏览器不支持 HTML5 视频，可以<a href="./media/poker-introduction.mp4">直接下载观看</a>。
  </video>
</div>

## 最新动态

不定期更新使用案例和功能说明。

{% for post in site.posts limit:3 %}
- [{{ post.title }}]({{ post.url | relative_url }}) · {{ post.date | date: "%Y-%m-%d" }}
{% endfor %}

[查看全部动态 →](./blog/)

## 全部篇幅

| # | 主题 | 你会读到什么 |
|---|---|---|
| 01 | [盲注时钟](./01-clock.html) | 大屏上的倒计时为什么可信，切后台、暂停、刷新都不会漂 |
| 02 | [赛事管理](./02-tournament.html) | 从空白到开赛，一场比赛要做的几步 |
| 03 | [终端配置](./03-terminal.html) | 怎么把客厅电视、投影、副屏变成赛事大屏 |
| 04 | [俱乐部规模方案](./04-scale.html) | 家庭局、小型俱乐部、多桌场分别怎么配 |
| 05 | [新用户试用](./05-trial.html) | 1 台设备 + 1 场赛事 + 3 天，够不够用 |
| 06 | [主题与视觉](./06-themes.html) | 大屏长什么样，能改到什么程度 |
| 07 | [语音播报](./07-voice.html) | 升盲提醒是谁在念、念什么、能不能关 |
| 08 | [计分与图例](./08-chips.html) | 屏幕下方那排筹码，颜色和面值怎么定 |
| 09 | [多屏同步](./09-realtime.html) | 主屏和副屏为什么能保持一致 |
| 10 | [团队协作](./10-permissions.html) | 老板、店长、荷官、观众分别能做什么 |
| 11 | [常见问题](./11-faq.html) | 断网、电视浏览器、续期、数据丢失等实际疑问 |

---

[从第一篇开始：盲注时钟 →](./01-clock.html)
