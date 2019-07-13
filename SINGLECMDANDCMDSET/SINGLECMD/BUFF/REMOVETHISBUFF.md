
%RemoveThisBuff

；2019/5/10 下午 8:59:49

[ 导航链接列表

/*Nav*/

]
# RemoveThisBuff 指令

##描述
移除这个 buff 指定层数。
参数为整数，要移除的层数。
只可以和事件连用。详情参考 `事件`。
；TODO： 以后换成链接

##参数

｜序号｜ 参数 ｜是否可选｜          描述  ｜
｜:--:｜:----:｜:------:｜:--------:｜
｜1  ｜ 整数，移除的层数 ｜   是   ｜ 要移除的层数；<br/>为空则移除一层｜


##示例
### excel-Card 表格
｜参考列｜    表头    ｜ 值 ｜
｜:----:｜:----------:｜:--:｜
｜  A   ｜     id     ｜ 150(请根据实际情况填写)   ｜
｜  B   ｜displayName ｜  测试Buff  ｜
｜…略…｜            ｜    ｜
｜  M   ｜    code    ｜ evt.StartTurn:{RemoveThisBuff:}  ｜
｜…略…｜            ｜    ｜


｜参考列｜    表头    ｜ 值 ｜
｜:----:｜:----------:｜:--:｜
｜  A   ｜     id     ｜ 151(请根据实际情况填写)   ｜
｜  B   ｜displayName ｜  测试卡牌  ｜
｜…略…｜            ｜    ｜
｜  M   ｜    code    ｜ AddBuff:150   ｜
｜…略…｜            ｜    ｜
**结果：id 为 150 的 buff 会在回合开始时自动移除**
![RemoveThisBuffSample1](removethisbuff~/Images~/REMOVETHISBUFFSAMPLE1.png)
![RemoveThisBuffSample2](removethisbuff~/Images~/REMOVETHISBUFFSAMPLE2.png)
##注意
+ `RemoveThisBuff` 指令只能和事件连用！