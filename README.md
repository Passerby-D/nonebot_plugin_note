
# 介绍

这是一个有提醒功能的记事本~  

# 安装

## pip 
`pip install nonebot_plugin_note`

## nb_cli
`nb plugin install nonebot_plugin_note`

# 使用
`nonebot.load_plugin('nonebot_plugin_note')`


# 命令

输入命令'note/记事/记事本 [记事内容]'进行记事  
输入命令'interval_note/间隔记事/间隔记事本 [记事内容] [时] [分] [秒]'，我将每隔[时][分][秒]提醒您一次  
输入命令'cron_note/定时记事/定时记事本 [记事内容] （日）/（mon/tue/wed/thu/fri/sat/sun） （[时]） （[分]） [秒]'，我将在每月的[日][时][分][秒]/每周的[星期x][时][分][秒]/每天的[时][分][秒]/每时的[分][秒]/每分的[秒]提醒您一次  
输入命令'date_note/单次记事/单次记事本 [记事内容] [年] [月] [日]（或今天/明天/后天/大后天） [时] [分] [秒]'，我将在这个时刻提醒您  
输入命令'note_list/记事列表/记事本列表'来查看记事列表  
输入命令'note_delete/记事删除/记事本删除 [记事内容]'来删除一个记事项目      
以下命令需要SUPERUSERS才能使用：  
输入命令'note_check/记事查看/记事本查看 [QQ账号]/all'来查看某人/所有的记事项目  
输入命令'note_remove/记事移除/记事本移除 [QQ账号] [记事内容]'来移除某人的某项记事内容  
输入命令'note_spy/记事监控/记事本监控 [QQ账号]'来监控某人的记事记录  
输入命令'note_spy_remove/记事监控移除/记事本监控移除 [QQ账号]'来移除对某人的监控  
输入命令'note_ban/记事禁止/记事本禁止 1/2（word/user） [内容]'来设置禁用词/黑名单  
输入命令'note_ban_list/记事禁止列表/记事本禁止列表'来查看禁用词和黑名单  
输入命令'note_ban_remove/记事禁止移除/记事本禁止移除 1/2（word/user） [内容]'来移除禁用词/黑名单      

# 🐦 TODO list

- [x]黑名单
- [x]监控某人记事
- [x]改为根据文字生成图片回复
- [ ]cron_note和date_note时不回复就会过一段时间再提醒一下
- [ ]
- [ ]
- [ ]
- [ ]
