# 规范细节

> 如果你要认领我们翻译的任务，并成为对应字幕的贡献者，希望你能认真阅读一下这里的规范细节，保证步调的统一。

## 1 概述
你从每个课时中拿到的，有YouTube语音识别自动生成的英文字幕，还有我们抽取的整个讲稿。
当认领了某一个单元，你就可以按照如下流程，高效统一地开始MIT6.824的翻译了！
当然，欢迎加入我们字幕组的QQ群，与更多志同道合的小伙伴一起交流，共同进步！（群号：1035287657）

## 2 分布式翻译

### 2.1 基本思想
为了提高大家的效率，建议大家尽可能借助机翻，为了提高机翻的准确性，需要大家对汇总的整个讲稿，断句、去掉一些语气词，还有更重要的，纠正机器生成的字幕的错误（记得同步到英文字幕文件中哦）。
之后，为了翻译像一个老师讲课的效果，需要你在完成机翻后，完整地边听边润色，注意一些术语的翻译，我们在doc中添加了一个中文书籍中的术语表，作为基本参考。更多不熟悉的术语，欢迎进入翻译群讨论。
这一步翻译的输入输出，我们下面就来仔细介绍~

### 2.2 翻译流程
#### 输入文件
机器生成英文字幕 + 英文字幕汇总后的完整讲稿
#### 输出文件
修改后的英文字幕 + 语义断句后的英文讲稿 + 机翻并润色的中文讲稿

#### 翻译建议流程
1. 经过认真的听课与对照，你会对上面两文件中的错误进行调整，为了方便讲稿的机翻，你可以去掉讲稿中的一些语气词，并按照语义断句（长的句子可能比较难断，后面我们会有一些建议，辅助你）
2. 断句修改后的文件保存（作为输出之一），使用Chrome或谷歌翻译，进行机翻。
3. 但是机翻的效果可能不会特别好，你需要根据一些口语习惯，特定术语，进行调整；机翻之后也能帮助你发现之前步骤的错误，回过头，继续修改字幕文件和英文讲稿。

#### 输出输出规范
**文件命名：**
按照每个单元 如自己负责的 Lecx 的第 y 个单元，断句后英语讲稿部分上传
Lecx-y.en.txt；断句后中文翻译上传Lecx-y.zh.txt；原srt修正后并入Lecx
.en.srt。（边界划分原则为向下断句，比如某一行9:59-10:01，属于第一个

最后我们会统一合并，生成Lecx.zh.srt和Lecx.srt

#### 输入输出文件举例
**原始 srt 文件**(截取自 lec07/tolerance_raft_2.en.srt)：
```
807
00:40:53,140 --> 00:40:55,690
to move the arm the right track right so

808
00:40:55,690 --> 00:40:58,570
these persistance can be terribly

809
00:40:58,570 --> 00:41:01,510
terribly expensive and if for sort of

810
00:41:01,510 --> 00:41:03,520
any kind of straightforward design

811
00:41:03,520 --> 00:41:06,220
they’re likely to be the limiting factor

812
00:41:06,220 --> 00:41:09,089
in performance because they mean that

813
00:41:09,089 --> 00:41:13,690
doing anything anything whatsoever on

814
00:41:13,690 --> 00:41:15,339
these Raft servers takes ten

815
00:41:15,339 --> 00:41:18,580
milliseconds a pop and 10 milliseconds
```

**汇总后的讲稿（如Lec7.en.txt）**
```
so these persistence can be terribly terribly expensive and if for sort of any kind of straightforward design they’re likely to be the limiting factor in performance because they mean that doing anything anything whatsoever on these Raft servers takes ten milliseconds a pop 
```

**修正机器生成字幕错误后字幕并入（Lec7.en.srt）**
>同输入

**英文断句后输出（Lec7-1.en.txt）**
```
so these persistence can be terribly terribly expensive
and if for sort of any kind of straightforward design
they’re likely to be the limiting factor in performance
because they mean that doing anything 
anything whatsoever on these Raft servers takes ten milliseconds a pop 
```
**机翻润色中文输出（Lec7-1.zh.txt）**
```
所以这些持久化的代价可能会非常大
如果只是用于一个简单的设计
它们可能成为性能的限制因素
因为这意味着做任何事情 
这些Raft服务器上的所有内容都会花费10毫秒的时间
......
```

#### 注意事项
1. 输入英文字幕为机器转语音，可能会有错误
2. 修改后的英文字幕时间轴不变，只是修改一些错误
3. 修改的时候，可能会有信息冗余（英文字幕与讲稿之间），所以注意两文件间同步

#### 分工
通常一个小任务为 5min，或者 10min，在项目中新建立一个 issue，标题为 "lec04;20-30min"，根据自己的实际情况选择。
完成小任务后，一定要及时发起 pr，合入之后，你就可以关闭你的 issue 了。

#### 技巧推荐
1. 对于长句（@鱼蛋是我我是橘猫）：使用谷歌对汇总后的讲稿直接翻译，谷歌会帮助去掉语气词，用来辅助断句。
2. 机翻直接采用Chrome打开后翻译（无字数限制）/Google translate（有字数限制）


## 3 字幕校正

这部分工作你不用担心，我们字幕组会有专门的同学针对完整的字幕文件做统一的修正。当然，如果你在观看过程中，发现有地方翻译的不对，请及时纠正，并提 PR.

## 最后，感谢每一个贡献者的参与！