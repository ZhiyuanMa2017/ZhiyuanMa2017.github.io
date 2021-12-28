---
layout: post
title: Delete or hide Wechat Icon in macOS menu bar
tags:
  - weixin
  - 微信
  - wechat
  - macOS
  - Mac
  - MacBook Pro
---
删除或隐藏Mac上微信状态栏图标

Applications  \> WeChat.app \> Contents \> Resources

Then delete **Assets.car**

**Update:**  

I found the previous solution not working very well. Though no Wechat icon in menu bar, there is still a placeholder and it will show numbers when you receive new messages.  

So, try [Dozer](https://github.com/Mortennn/Dozer), move the icons you want to hide to the left of the Dozer icon, and then enable *Hide both Dozer icons when status bar are hidden*. You will not see the annoying Wechat icon anymore.
