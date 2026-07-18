---
title: Windows全盘迁移后，新旧机的Tailscale登录态冲突 # 在线VS Code可以看到Front Matter是否能被正确解析
date: 2025-11-21 23:07:24 +0800 # YYYY-MM-DD HH:MM:SS +0800
categories: [技术博客, 电脑] # 可以加三级目录名，但分类那个页面只会显示到二级
tags: [Windows,系统迁移,Tailscale]     # TAG names should always be lowercase，但我用标签大写也能正常显示
---

>事情实际大概发生在2025年11月21日前后，于2026年7月18日回忆写下。
{: .prompt-info }

此事在古籍（doge）亦有记载：
[换机迁移后Localsend新旧手机无法互相识别？重装应用即可 | KenXK](https://kenxk.github.io/posts/%E6%8D%A2%E6%9C%BA%E8%BF%81%E7%A7%BB%E5%90%8ELocalsend%E6%96%B0%E6%97%A7%E6%89%8B%E6%9C%BA%E6%97%A0%E6%B3%95%E4%BA%92%E7%9B%B8%E8%AF%86%E5%88%AB-%E9%87%8D%E8%A3%85%E5%BA%94%E7%94%A8%E5%8D%B3%E5%8F%AF/)

具体情景就是用Dism++把整个系统分区备份，在新机子上还原出来。然后发现新旧电脑上的Tailscale只能登录其中一个，尝试同时登录的话好像是会把先登录的那个踢下线，在Tailscale控制台改名也没用。

猜想是标识符基于旧机子（系统）生辰，迁移过程带过来了。忘了重装能不能解决，因为旧机子迁移完就丢一边不再用了，所以对我来说问题解决了就没有再研究。