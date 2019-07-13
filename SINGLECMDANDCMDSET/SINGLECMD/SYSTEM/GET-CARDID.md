
%get_cardId

；2019/5/10 上午 11:45:31
[ 导航链接列表

/*Nav*/

]
# get_cardId 指令

##描述
获取执行指令的卡牌 id。
返回值为字符串。
常用在指令组。
##参数

<1.2>无参数



##示例
#### excel-Card 表格

｜参考列｜    表头    ｜ 值 ｜
｜:----:｜:----------:｜:--:｜
｜  A   ｜     id     ｜ 150(请根据实际情况填写)   ｜
｜  B   ｜displayName ｜  测试Buff  ｜
｜…略…｜            ｜    ｜
｜  M   ｜    code    ｜ evt.StartTurn:{If:{<:{ThisBuffCount:},2},{TakeDamage:1},{Heal:1}} ｜
｜…略…｜            ｜    ｜

｜参考列｜    表头    ｜ 值 ｜
｜:----:｜:----------:｜:--:｜
｜  A   ｜     id     ｜ 151(请根据实际情况填写)   ｜
｜  B   ｜displayName ｜  测试卡牌  ｜
｜…略…｜            ｜    ｜
｜  M   ｜    code    ｜ AddBuff:150  ｜
｜…略…｜            ｜    ｜
### excel-CardCommand 表格
｜参考列｜    表头    ｜ 值 ｜
｜:----:｜:----------:｜:--:｜
｜  A   ｜     id     ｜  ThisBuffCount  ｜
｜  B   ｜description ｜ 这个 buff 数目   ｜
｜…略…｜            ｜    ｜
｜  M   ｜    code    ｜  BuffCount:{get_cardId:}  ｜
｜…略…｜            ｜    ｜

**结果：每次回合开始，如果这个 buff(id 为150) 的数目小于 2 就受到 1 点伤害，否则就回复 1 点 HP。**
![get-cardIdSample1](get-cardid~/Images~/GET-CARDIDSAMPLE1.png)
<br/>
> *技巧：* 使用 `变量语法糖` 可增加代码易读性，详情可参考 `变量语法糖 $`。

；TODO: 以后改为链接

##注意
+`get_cardId` 指令返回值为字符串。

