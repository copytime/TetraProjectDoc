
%ConvertBuff

；2019/5/10 下午 11:13:30
[ 导航链接列表

/*Nav*/

]
# ConvertBuff 指令

##描述
将指定层数指定 id 的 buff 转化为指定层数指定 id 的另一个 buff。
参数一为被转换的 buff id。
参数二为被转换的 buff 层数。
参数三为转换目标的 buff id。
参数二为转换目标的 buff 层数。
##参数

｜序号｜ 参数 ｜是否可选｜          描述  ｜
｜:--:｜:----:｜:------:｜:--------:｜
｜1  ｜ 字符串，buff id ｜   否   ｜ 被转换的 buff id｜
｜2 ｜ 整数，层数 ｜   否   ｜ 被转换的 buff 层数｜
｜3  ｜ 字符串，buff id ｜   否   ｜ 转换目标的 buff id｜
｜4 ｜ 整数，层数 ｜   否   ｜ 转换目标的 buff 层数｜
##示例
#### excel-Card 表格
｜参考列｜    表头    ｜ 值 ｜
｜:----:｜:----------:｜:--:｜
｜  A   ｜     id     ｜ 150(请根据实际情况填写)   ｜
｜  B   ｜displayName ｜  测试卡牌  ｜
｜…略…｜            ｜    ｜
｜  M   ｜    code    ｜  ConvertBuff:41,3,83,1 ｜
｜…略…｜            ｜    ｜

**结果：把 3 层 id 为 41 的 buff 转化为 1 层 id 为 83 的 buff**
![ConvertBuffSample1](convertbuff~/Images~/CONVERTBUFFSAMPLE1.png)
