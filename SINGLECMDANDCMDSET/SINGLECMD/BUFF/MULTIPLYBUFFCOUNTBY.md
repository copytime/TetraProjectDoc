
%MultiplyBuffCountBy

；2019/5/10 下午 10:59:32
[ 导航链接列表

/*Nav*/

]
# MultiplyBuffCountBy 指令

##描述
将指定 buff 数目乘以指定系数。
参数一为 buff 的 id ，参数二为指定的系数。

##参数

｜序号｜ 参数 ｜是否可选｜          描述  ｜
｜:--:｜:----:｜:------:｜:--------:｜
｜1  ｜ 字符串，buff id ｜   否   ｜ 要倍数的 buff 的 id｜
｜2 ｜ 浮点数，系数 ｜   否   ｜ 乘以的系数｜

##示例
###示例一：
#### excel-Card 表格
｜参考列｜    表头    ｜ 值 ｜
｜:----:｜:----------:｜:--:｜
｜  A   ｜     id     ｜ 150(请根据实际情况填写)   ｜
｜  B   ｜displayName ｜  测试卡牌  ｜
｜…略…｜            ｜    ｜
｜  M   ｜    code    ｜  MultiplyBuffCountBy:83,2 ｜
｜…略…｜            ｜    ｜

**结果：将目标身上 id 为 83 的 buff 数目乘以 2**
![MultiplyBuffCountBySample1](multiplybuffcountby~/Images~/MULTIPLYBUFFCOUNTBYSAMPLE1.png)