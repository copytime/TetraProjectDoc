
%AddBuff

；2019/5/10 下午 11:31:12
[ 导航链接列表

/*Nav*/

]
# AddBuff 指令

##描述
添加指定 buff 指定层数。
参数一为指定 buff id，参数二为指定添加的层数。
；TODO： 增加对 Character 类里面有三个参数的 addBuff 的描述
##参数

｜序号｜ 参数 ｜是否可选｜          描述  ｜
｜:--:｜:----:｜:------:｜:--------:｜
｜1  ｜ 整数，buff id ｜   否   ｜ 要添加的 buff｜
｜2 ｜ 整数，层数 ｜   否   ｜ 要添加的层数｜


##示例
### excel-Card 表格
｜参考列｜    表头    ｜ 值 ｜
｜:----:｜:----------:｜:--:｜
｜  A   ｜     id     ｜ 150(请根据实际情况填写)   ｜
｜  B   ｜displayName ｜  测试卡牌  ｜
｜…略…｜            ｜    ｜
｜  M   ｜    code    ｜ AddBuff:83,3  ｜
｜…略…｜            ｜    ｜

**结果：添加 id 为 83 的 buff 3 层**
![AddBuffSample1](addbuff~/Images~/ADDBUFFSAMPLE1.png)
