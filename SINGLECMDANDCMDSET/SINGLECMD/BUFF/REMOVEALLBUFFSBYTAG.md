
%RemoveAllBuffsByTag

；2019/5/10 下午 9:35:41
[ 导航链接列表

/*Nav*/

]
# RemoveAllBuffsByTag 指令

##描述
移除全部或指定层数的指定 tagCode 的 buff。
参数一为 buff 的 tagCode ，参数二为指定移除的层数。

##参数

｜序号｜ 参数 ｜是否可选｜          描述  ｜
｜:--:｜:----:｜:------:｜:--------:｜
｜1  ｜ 字符串，tagCode ｜   否   ｜ 要移除的 buff 的 tagCode｜
｜2 ｜ 整数，层数 ｜   是   ｜ 要移除的层数；<br/>若为空则全部移除｜

##示例
###示例一：
#### excel-Card 表格
｜参考列｜    表头    ｜ 值 ｜
｜:----:｜:----------:｜:--:｜
｜  A   ｜     id     ｜ 150(请根据实际情况填写)   ｜
｜  B   ｜displayName ｜  测试卡牌  ｜
｜…略…｜            ｜    ｜
｜  M   ｜    code    ｜  RemoveAllBuffsByTag:Debuff ｜
｜…略…｜            ｜    ｜

**结果：移除所有的 tagCode 为 Debuff 的 buff**
###示例二：
#### excel-Card 表格
｜参考列｜    表头    ｜ 值 ｜
｜:----:｜:----------:｜:--:｜
｜  A   ｜     id     ｜ 150(请根据实际情况填写)   ｜
｜  B   ｜displayName ｜  测试卡牌  ｜
｜…略…｜            ｜    ｜
｜  M   ｜    code    ｜  RemoveAllBuffsByTag:Debuff,2 ｜
｜…略…｜            ｜    ｜

**结果：移除所有的 tagCode 为 Debuff 的 buff 2 层**

