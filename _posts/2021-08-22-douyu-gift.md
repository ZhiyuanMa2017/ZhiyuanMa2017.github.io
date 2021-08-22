---
layout: post
title: Douyu send gift javascript code
tags:
  - League of Legends
  - douyu
  - script
---
斗鱼送礼物脚本
propId 礼物ID，268 荧光棒  
YourRoomID 填入想送的房间号

```javascript
const timer = ms=>new Promise(res=>setTimeout(res, ms))
async function load() {
    var i = 0;
    while (i < 60) {
        await timer(100);
        i++;
        console.log(i);
        let formData = new FormData();
        formData.append("propId", "268");
        formData.append("propCount", 1);
        formData.append("roomId", YourRoomID);
        fetch('https://www.douyu.com/japi/prop/donate/mainsite/v1', {
            method: 'POST',
            body: formData
        }).then(res=>res.json()).then(res=>{
            if (res && 'error'in res && res.error === 0) {
                console.log('成功赠送主播 : ' + YourRoomID + ' 一个荧光棒');
            } else {
                console.log('赠送失败 : ' + res.msg);
            }
        }
        );
    }

}

load();

```
