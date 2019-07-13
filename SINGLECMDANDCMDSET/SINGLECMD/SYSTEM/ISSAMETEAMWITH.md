
%IsSameTeamWith

；2019/5/10 下午 2:49:53

[ 导航链接列表

/*Nav*/

]
# IsSameTeamWith 指令

##描述
判断角色是否和指定角色同一队伍。
参数为角色(Character类)，使用者和目标可以是同一人，即：自己可以和自己是同一队伍。
返回值为布尔值。
##参数


｜序号｜ 参数 ｜是否可选｜          描述  ｜
｜:--:｜:----:｜:------:｜:--------:｜
｜1  ｜ 角色(Character类) ｜   否   ｜指定角色｜


##示例
### excel-Card 表格

｜参考列｜    表头    ｜ 值 ｜
｜:----:｜:----------:｜:--:｜
｜  A   ｜     id     ｜  150(请根据实际情况填写) ｜
｜  B   ｜displayName ｜  测试卡牌  ｜
｜…略…｜            ｜    ｜
｜  M   ｜    code    ｜  If:{tgt.IsSameTeamWith:$user},{Heal:1},{TakeDamage:1} ｜
｜…略…｜            ｜    ｜

**结果：如果目标和使用者在同一队伍里就回复 1 点 HP，否则造成 1 点伤害**
![IsSameTeamWithSample1](issameteamwith~/Images~/ISSAMETEAMWITHSAMPLE1.png)
##注意
+ 使用者和目标可以是同一人，即：自己可以和自己是同一队伍。