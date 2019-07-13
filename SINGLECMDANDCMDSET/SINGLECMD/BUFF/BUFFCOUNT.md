
%BuffCount 和 GetBuffCount

；2019/5/10 下午 11:25:47
[ 导航链接列表

/*Nav*/

]
# BuffCount 指令

##描述
`BuffCount` 为 `GetBuffCount` 关键字的缩写，两者作用一致。
返回指定 id 的 buff 层数。
参数为 buff 的 id。

##参数

｜序号｜ 参数 ｜是否可选｜          描述  ｜
｜:--:｜:----:｜:------:｜:--------:｜
｜1  ｜ 字符串，buff id ｜   否   ｜ 要获取层数的 buff 的 id｜

##示例
#### excel-Card 表格
｜参考列｜    表头    ｜ 值 ｜
｜:----:｜:----------:｜:--:｜
｜  A   ｜     id     ｜ 150(请根据实际情况填写)   ｜
｜  B   ｜displayName ｜  测试卡牌  ｜
｜…略…｜            ｜    ｜
｜  M   ｜    code    ｜  If:{==:{tgt.BuffCount:83},1},{Heal:1},{TakeDamage:1}｜
｜…略…｜            ｜    ｜

**结果：如果目标 id 为 83 的 buff 层数为 1，就回复 1 点 HP，否则就造成 1 点伤害**
![BuffCountSample1](buffcount~/Images~/BUFFCOUNTSAMPLE1.png)
