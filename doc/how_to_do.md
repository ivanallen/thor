# 如何翻译

## 1 快速开始

例如，这是一个原始的 srt 文件(截取自 lec03/gfs.srt)：

```
10
00:00:31,410 --> 00:00:34,260
abstraction you might you know if you

11
00:00:34,260 --> 00:00:35,850
didn't know already you might imagine

12
00:00:35,850 --> 00:00:37,230
that there could be all kinds of

13
00:00:37,230 --> 00:00:40,050
different you know important

14
00:00:40,050 --> 00:00:42,030
abstractions you might want to use for

15
00:00:42,030 --> 00:00:43,650
distributed systems but it's turned out

16
00:00:43,650 --> 00:00:47,730
that a simple storage interface is just

17
00:00:47,730 --> 00:00:50,010
incredibly useful and extremely general
```

翻译之后，会变成这样：

```
10
00:00:31,410 --> 00:00:34,260
因为存储被证明是一种关键抽象
abstraction you might you know if you

11
00:00:34,260 --> 00:00:35,850
如果你还不知道的话
didn't know already you might imagine

12
00:00:35,850 --> 00:00:37,230
你可以想象在分布式系统中
that there could be all kinds of

13
00:00:37,230 --> 00:00:40,050
你希望使用的各种不同的抽象
different you know important

14
00:00:40,050 --> 00:00:42,030
你希望使用的各种不同的抽象
abstractions you might want to use for

15
00:00:42,030 --> 00:00:43,650
但事实表明
distributed systems but it's turned out

16
00:00:43,650 --> 00:00:47,730
简单的存储接口往往更有用而且更加通用
that a simple storage interface is just

17
00:00:47,730 --> 00:00:50,010
简单的存储接口往往更有用而且更加通用
incredibly useful and extremely general
```

你直接修改 gfs.srt 即可。如果你不放心，你可备份一个 gfs.srt，自己再单独创建一个 gfs2.srt。

## 2 翻译技巧

你可以使用谷歌翻译工具进行批量翻译，这样可以帮助你提高翻译效率。当然，我们正在制作自动化工具，让你第一手拿到的原始 srt 就已经包含了机翻结果，这样你只需要修正就可以了。

如果有些英文长句太长，而中文更加紧凑，可以把中文多复制几份，每个时间轴都放上一样的翻译。可以参考第 1 节的示例。

## 3 怎么知道自己翻译的部分和别人是否冲突

解决方案很简单，新建立一个 issue，标题为 "lec04;20-30min"，同时把这个任务分配给自己，这样就不会有人和你翻译冲突了。

通常一个小任务为 5min，或者 10min，根据自己的实际情况选择。完成小任务后，一定要及时发起 pr，合入之后，你就可以关闭你的 issue 了。

## 4 字幕校正

这部分工作你不用担心，会有专门的同学针对完整的字幕文件做统一的修正。当然，如果你在观看过程中，发现有地方翻译的不对，请及时纠正，并提 PR.
