
%HasBuff

；2019/5/10 下午 11:06:34
[ 导航链接列表

/*Nav*/

]
# HasBuff 指令

##描述
目标指定 buff 是否大于等于指定层数。
可用来判断目标是否有指定 buff。
参数一为 buff 的 id ，参数二为指定的层数。
返回值为布尔值。

##参数

｜序号｜ 参数 ｜是否可选｜          描述  ｜
｜:--:｜:----:｜:------:｜:--------:｜
｜1  ｜ 字符串，buff id ｜   否   ｜ 要判断的 buff 的 id｜
｜2 ｜ 整数，层数 ｜   是   ｜ 返回指定 buff 层数是否大于等于指定层数；<br/>若为则返回目标是否有指定 buff｜

##示例
###示例一：
#### excel-Card 表格
｜参考列｜    表头    ｜ 值 ｜
｜:----:｜:----------:｜:--:｜
｜  A   ｜     id     ｜ 150(请根据实际情况填写)   ｜
｜  B   ｜displayName ｜  测试卡牌  ｜
｜…略…｜            ｜    ｜
｜  M   ｜    code    ｜  If:{tgt.HasBuff:83},{Heal:1},{TakeDamage:1}｜
｜…略…｜            ｜    ｜

**结果：如果目标有 id 为 83 的 buff，就回复 1 点 HP，否则就造成 1 点伤害**
###示例二：
#### excel-Card 表格
｜参考列｜    表头    ｜ 值 ｜
｜:----:｜:----------:｜:--:｜
｜  A   ｜     id     ｜ 150(请根据实际情况填写)   ｜
｜  B   ｜displayName ｜  测试卡牌  ｜
｜…略…｜            ｜    ｜
｜  M   ｜    code    ｜  If:{tgt.HasBuff:83,3},{Heal:1},{TakeDamage:1} ｜
｜…略…｜            ｜    ｜

**结果：如果目标的 id 为 83 的 buff 层数大于等于 3，就回复 1 点 HP，否则就造成 1 点伤害**
