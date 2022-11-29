<div align="center">
  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
  <br>
  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
</div>

<div align="center">

# nonebot_plugin_note
  
_✨ NoneBot 一个有提醒功能的记事本插件  ✨_
  
<a href="https://pypi.python.org/pypi/nonebot-plugin-note">
    <img src="https://img.shields.io/pypi/v/nonebot-plugin-note.svg" alt="pypi">
</a>

</div>


# 安装

* pip 
```
pip install nonebot_plugin_note
```

* nb_cli
```
nb plugin install nonebot_plugin_note
```

# 配置.env

```
# nonebot_plugin_note
NOTE_FONT_COLOR=[149,98,49] # 笔记文字颜色
NOTE_BG_COLOR=[255,245,151] # 笔记背景颜色
```

# 使用
```
nonebot.load_plugin('nonebot_plugin_note')
```


# 命令
**注：使用命令时需要加命令前缀**（举例中的命令前缀为 /，请根据情况替换）

* `note/记事/记事本 [记事内容]` 进行记事  
例如：`/记事 这里记录自己的一件事情，后期可以通过记事列表命令查看，记事删除命令删除`  

* `interval_note/间隔记事/间隔记事本 [记事内容] [时] [分] [秒]`，我将每隔[时][分][秒]提醒您一次  
例如：`/间隔记事 后面是时分秒，时分秒之间有空格，每隔一个周期提醒，比如这个010就是每隔1分钟提醒一次 0 1 0`  

* `cron_note/定时记事/定时记事本 [记事内容] （日）/（mon/tue/wed/thu/fri/sat/sun） （[时]） （[分]） [秒]`，我将在每月的[日][时][分][秒]/每周的[星期x][时][分][秒]/每天的[时][分][秒]/每时的[分][秒]/每分的[秒]提醒您一次  
例如：
`/定时记事 每周的tue(星期二)日0时24分0秒提醒 tue 0 24 0`  
`/定时记事 每月的29日0时26分0秒提醒 29 0 26 0 `  
`/定时记事 每时的26分50秒提醒 26 50  `  
`/定时记事 每分的26秒提醒 26 `  

* `date_note/单次记事/单次记事本 [记事内容] [年] [月] [日]（或今天/明天/后天/大后天） [时] [分] [秒]`，我将在这个时刻提醒您  
例如：  
`/单次记事 将在2022年11月29日0时31分0秒提醒 2022 11 29 0 31 00`  
`/单次记事 将在2022年11月29日0时32分10秒提醒(今天就是这个日子) 今天 0 32 10 `

* `note_list/记事列表/记事本列表` 来查看记事列表  
例如：`/记事列表`  

* `note_delete/记事删除/记事本删除 [记事内容]` 来删除一个记事项目    
例如：`/记事删除 这里记录自己的一件事情，后期可以通过记事列表命令查看，记事删除命令删除`    



以下命令需要SUPERUSERS才能使用：  

* `note_check/记事查看/记事本查看 [QQ账号]/all` 来查看某人/所有的记事项目  
例如：`/记事查看 all`  
`/记事查看 123456`  

* `note_remove/记事移除/记事本移除 [QQ账号] [记事内容]` 来移除某人的某项记事内容  
例如：`/记事移除 123456 记事内容`    

* `note_spy/记事监控/记事本监控 [QQ账号]` 来监控某人的记事记录  
例如：`/note_spy 123456`  

* `note_spy_remove/记事监控移除/记事本监控移除 [QQ账号]` 来移除对某人的监控  
例如：`/记事本监控移除 123456`  

* `note_ban/记事禁止/记事本禁止 1/2（word/user） [内容]` 来设置禁用词/黑名单  
例如：`/记事禁止 1 1表示禁止的记事内容`  
`/记事禁止 2 123456`  

* `note_ban_list/记事禁止列表/记事本禁止列表` 来查看禁用词和黑名单  
例如：`/记事禁止列表`   

* `note_ban_remove/记事禁止移除/记事本禁止移除 1/2（word/user） [内容]` 来移除禁用词/黑名单  
例如：`/记事禁止移除 1表示移除禁止的记事内容`  
`/记事禁止移除 2 123456`  

# 其他

有bug有什么想法都可以告诉我，鄙人qq：850199308

# 🐦 TODO list

- [x] 黑名单
- [x] 监控某人记事
- [x] 改为根据文字生成图片回复
- [ ] cron_note和date_note时不回复就会过一段时间再提醒一下

