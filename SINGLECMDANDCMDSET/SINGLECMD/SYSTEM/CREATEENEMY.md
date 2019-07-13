
%CreateEnemy

；2019/5/10 上午 8:37:08

[ 导航链接列表

/*Nav*/

]
# CreateEnemy 指令

##描述
在指定位置生成一个指定角色的敌人角色。
敌人角色会主动攻击玩家角色。
敌人角色在 `tagCode` 为 `Main` 时敌人的 AI 不会运作。
##参数



｜序号｜ 参数 ｜是否可选｜          描述  ｜
｜:--:｜:----:｜:------:｜:--------:｜
｜1  ｜ 角色 id ｜   否   ｜要设为敌人的角色 id ｜
｜1  ｜ 三维向量，位置信息 ｜   否   ｜要生成敌人的位置 ｜



##示例
###示例一：
#### excel-Card 表格

｜参考列｜    表头    ｜ 值 ｜
｜:----:｜:----------:｜:--:｜
｜  A   ｜     id     ｜  150(请根据实际情况填写) ｜
｜  B   ｜displayName ｜  测试卡牌  ｜
｜…略…｜            ｜    ｜
｜  M   ｜    code    ｜  CreateEnemy:1,{get_selectedPosition:}  ｜
｜…略…｜            ｜    ｜

**结果：在选定位置生成角色 id 为 1 的敌人，此时由于角色的 `tagCode` 为 `Main` 所以生成的敌人 AI 不会运作**
![CreatEnemySample1](createenemy~/Images~/CREATENEMYSAMPLE1.png)
![CreatEnemySample2](createenemy~/Images~/CREATENEMYSAMPLE2.png)
###示例二：
｜参考列｜    表头    ｜ 值 ｜
｜:----:｜:----------:｜:--:｜
｜  A   ｜     id     ｜  150(请根据实际情况填写) ｜
｜  B   ｜displayName ｜  测试卡牌  ｜
｜…略…｜            ｜    ｜
｜  M   ｜    code    ｜  CreateEnemy:10,{get_selectedPosition:}  ｜
｜…略…｜            ｜    ｜

**结果：在选定位置生成角色 id 为 10 的敌人，此时敌人会由 AI 自动运作**

##注意
+ `CreateEnemy` 指令生成的敌人如果角色的 `tagCode` 为 `Main` 的话，AI 是不会运作的。


