
%CreateTeammate

；2019/5/10 上午 10:54:06

[ 导航链接列表

/*Nav*/

]
# CreateTeammate 指令

##描述
在指定位置生成一个指定角色的队友角色。
队友角色不可以被玩家切换操作，但是会主动攻击敌人角色。
##参数



｜序号｜ 参数 ｜是否可选｜          描述  ｜
｜:--:｜:----:｜:------:｜:--------:｜
｜1  ｜ 角色 id ｜   否   ｜要设为中立角色的角色 id ｜
｜1  ｜ 三维向量，位置信息 ｜   否   ｜要生成中立角色的位置 ｜



##示例
###示例一：
#### excel-Card 表格

｜参考列｜    表头    ｜ 值 ｜
｜:----:｜:----------:｜:--:｜
｜  A   ｜     id     ｜  150(请根据实际情况填写) ｜
｜  B   ｜displayName ｜  测试卡牌  ｜
｜…略…｜            ｜    ｜
｜  M   ｜    code    ｜  CreateEnemy:10,{get_selectedPosition:}  ｜
｜…略…｜            ｜    ｜

**结果：在选定位置生成角色 id 为 10 的队友角色**

<br/>
> *技巧：* 中立角色常常用来设置环境，比如 `油桶`、`黑洞` 等。

##注意
+ 队友角色不可以被玩家切换控制。