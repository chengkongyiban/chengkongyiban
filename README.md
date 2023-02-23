# 重写&规则集转换
欢迎加入群组https://t.me/zhangpeifu

欢迎订阅频道https://t.me/h5683577

## 安装地址:
   Surge LanceX [点击查看](https://raw.githubusercontent.com/chengkongyiban/Surge/main/modules/QX_to_Surge.sgmodule)  
   Shadowrocket [点击查看](https://raw.githubusercontent.com/chengkongyiban/shadowrocket/main/Block/QX_to_Shadowrocket.module)  
   Loon [点击查看](https://raw.githubusercontent.com/chengkongyiban/Loon/main/Loon-Gallery/Rewrite_to_Loon.plugin)  
   Stash [点击查看](https://raw.githubusercontent.com/chengkongyiban/stash/main/override_Store/Rewrite_to_Stash.stoverride)  
  
## 简介

支持将QX重写解析至Surge Shadowrocket Loon Stash  
  
支持将Surge模块解析至Shadowrock(仅需转换Mock为reject) Loon Stash  
  
支持5款代理app规则集互转  
  

## 如何使用:  
### 重写转换  
   Stash: 在QX重写链接末尾加qx.stoverride  在Surge模块链接末尾加sg.stoverride  
  
   Surge LanceX: 在QX重写链接末尾加qx  
  
   Shadowrock Loon: 在QX重写链接末尾加qx  在Surge模块链接末尾加sg  
  
### 规则集转换  
   在规则集链接末尾加r_parser.list  

## 参数说明  
### 重写转换  
   n=  修改名字+简介 ，名字和简介以"+"相连，可缺省名字或简介;  
   y=  根据关键词保留相关重写(即去掉注释) 多关键词以"+"相连  
   x=  根据关键词排除相关重写(即添加注释) 多关键词以"+"相连  
   i=  关闭随机插件图标(仅需传入i=即可 仅Loon需要此参数)  
   del= 从转换结果中剔除被注释的重写(仅需传入del=即可)  
   hnadd= 添加MITM主机名 多主机名以"+"相连  
   hndel= 从已有MITM主机名中删除主机名 多主机名以"+"相连(需要传入完整主机名)  
  
   在链接后加 "?" 使用参数, 不同参数用 "&" 连接  

   示例 https://raw.githubusercontent.com/chengkongyiban/shadowrocket/main/Block/bilibili.modulesg.stoverride?n=B站去广告+bilibili&y=魔改皮肤+Region&x=upos+简体字幕  

### 规则集转换  
   y=  根据关键词保留相关规则(即去掉注释) 多关键词以"+"相连  
   x=  根据关键词排除相关规则(即添加注释) 多关键词以"+"相连  
   nore=  为IP规则开启不解析域名(及no-resolve,仅需传入nore=)  

   示例 https://raw.githubusercontent.com/fmz200/wool_scripts/main/QuantumultX/filter/fenliu.listr_parser.list?x=baidu+jd&nore=  

## 关于需要开启binary-mode的脚本说明:  
   因为qx重写中对此类脚本没有特殊标记，仅能靠脚本名判断，如Maasea佬的YouTube去广告脚本没有以proto.js结尾，故转换后不会正确识别并开启  
   surge的可以正确识别并开启  

## 鸣谢  
原脚本作者@小白脸  
脚本修改[*@chengkongyiban*](https://github.com/chengkongyiban)  
感谢[*@xream*](https://github.com/xream) 提供的[replace-Header.js](https://github.com/xream/scripts/raw/main/surge/modules/replace-header/index.js)，[echo-response.js](https://github.com/xream/scripts/raw/main/surge/modules/echo-response/index.js)  
感谢[*@mieqq*](https://github.com/mieqq) 提供的[replace-body.js](https://github.com/mieqq/mieqq/raw/master/replace-body.js)  
插件图标用的 [*@Keikinn*](https://github.com/Keikinn) 的 [StickerOnScreen](https://github.com/KeiKinn/StickerOnScreen)项目，感谢  


<!--
**chengkongyiban/chengkongyiban** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
