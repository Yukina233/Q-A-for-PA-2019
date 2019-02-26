# Q&A for PA2019 NUAA

NUAA PA2019常见问题解答（持续更新，欢迎加星）

------

# 读前必看

1. 提问以前务必翻看翻看本问答文档，对于文档中已经给出的问题，助教均不再回复，敬请谅解！
2. 有偿（`1分钱QQ红包`）征集遇到的问题的解决办法
   想分享你遇到问题的解决办法？没问题你可以把想说的话，想提醒大家的事情，还包括代码框架本身的 bug 等等`直接以 Pull Requests 的形式`提交到本仓库的 `Master` 分支，遇到有人提交我会上去检查一下后合并的。另外这个问答的issue功能关掉了，以免有人使用不文明用语或发答案。
3. 请参与编写 Q&A 的同学严格按照[中文文案排版指北](https://github.com/sparanoid/chinese-copywriting-guidelines)排版，以减少维护工作量，谢谢！
4. 注意这里不是共享答案的地方，每周检查报告的时候是有查重的，请同学们珍惜自己的代码……因此遇到这种提交不予合并，技术性难题大家可以一起讨论。温馨提醒：每次提交的报告都会**查重**，请不要把自己的代码分享给别人，遇到**雷同的按讲义[课程设计提交要求](https://www.jinhangdev.cn/ics/text/others/submit-requirement.html#关于学术诚信)处理，敬请知晓！**
5. 新添加的问题将放在最前面，以免大家看不到以为没更新，想看历史比较久远的问题往后面看


# 关于手册勘误（很重要）

请务必看讲义的 `i386 手册勘误`部分，否则**实现指令出错将对后面的进程产生巨大负面影响，甚至导致无法继续往后做**，请务必留意！另外，有部分勘误是**直接**在 `i386 手册的 PDF 文件中`用`批注`形式标注出来的，**若你的PDF阅读器并不能看到这些*标记和批注*，请使用以下推荐的PDF阅读器**：[Adobe Reader](https://adobe-reader.en.softonic.com/)或[Adobe Acrobat](https://get.adobe.com/cn/reader/otherversions/)

---

# PA0

1. 安装虚拟机时遇到选择安装后黑屏，很可能是镜像文件本身的问题，请重新到 Debian 官网或者镜像点重新下载安装包镜像重新安装。

2. 有同学在nuaa.portal网络环境下发现无法用DHCP来配置网络，其原因是nuaa.portal不支持桥接，而拨号上网可以。解决方法是将虚拟机网卡1设置为NAT模式，网卡2设置为设置为仅主机网络(host-only)，之后重新用DHCP来配置网络即可上网。**（注意SSH需要使用host-only网卡的地址）**
