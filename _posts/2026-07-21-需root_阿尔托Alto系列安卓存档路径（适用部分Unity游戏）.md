---
title: 阿尔托Alto系列安卓存档路径（需root，适用部分Unity游戏） # 在线VS Code可以看到Front Matter是否能被正确解析
date: 2026-07-21 23:10:16 +0800 # YYYY-MM-DD HH:MM:SS +0800
categories: [技术博客,手机] # 可以加三级目录名，但分类那个页面只会显示到二级
tags: [存档,Unity,游戏,ROOT]     # TAG names should always be lowercase，但我用标签大写也能正常显示
---

用Unity做的游戏在Android平台上的默认存档路径是  
`/data/data/<包名>/shared_prefs/<包名>.v2.playerprefs.xml`{: .filepath}

比如阿尔托的冒险Alto's Adventure国际服（还是叫官服？相对于TapTap国服）就是  
`/data/data/com.noodlecake.altosadventure/shared_prefs/com.noodlecake.altosadventure.v2.playerprefs.xml`{: .filepath}

比如阿尔托的奥德赛Alto's Odyssey国际服（官服）就是  
`/data/data/com.noodlecake.odyssey/shared_prefs/com.noodlecake.odyssey.v2.playerprefs.xml`{: .filepath}

另外，本次存档迁移探索中，来源是第shan三zhai方重新包装（包名不是官服也不是TapTap国服，弹广告、霸道索要定位权限）的低版本，目标是官服的最新版。

![alt text](../assets/img/post/2026-07-21-安卓Unity存档路径/PixPin_2026-07-24_06-25-34.jpg){: .shadow}

![alt text](../assets/img/post/2026-07-21-安卓Unity存档路径/IMG_20260721_231016_1.jpg)

![alt text](../assets/img/post/2026-07-21-安卓Unity存档路径/IMG_20260722_001236.jpg)