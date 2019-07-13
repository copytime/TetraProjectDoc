
%RemoveBuff

；2019/5/10 下午 9:21:18
[ 导航链接列表

/*Nav*/

]
# RemoveBuff 指令

##描述
移除指定 buff 指定层数。
参数一为指定 buff id，参数二为指定移除的层数。

##参数

｜序号｜ 参数 ｜是否可选｜          描述  ｜
｜:--:｜:----:｜:------:｜:--------:｜
｜1  ｜ 整数，buff id ｜   否   ｜ 要移除的 buff｜
｜2 ｜ 整数，层数 ｜   否   ｜ 要移除的层数｜


##示例
### excel-Card 表格
｜参考列｜    表头    ｜ 值 ｜
｜:----:｜:----------:｜:--:｜
｜  A   ｜     id     ｜ 150(请根据实际情况填写)   ｜
｜  B   ｜displayName ｜  测试卡牌  ｜
｜…略…｜            ｜    ｜
｜  M   ｜    code    ｜ RemoveBuff:83,1  ｜
｜…略…｜            ｜    ｜

**结果：移除 id 为 83 的 buff 1 层**
![RemoveBuffSample1](removebuff~/Images~/REMOVEBUFFSAMPLE1.png)
