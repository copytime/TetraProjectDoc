
%ArgIsCard 和 IfArgIsCard

；2019/5/10 上午 12:24:22

[ 导航链接列表

/*Nav*/

]
# ArgIsCard 指令

##描述
`ArgIsCard` 和 `IfArgIsCard` 指令的作用一致。
加一个 If 只是为了更符合句子的语意。
判断事件传递的第一个参数是否是指定 id 的卡牌。
参数为卡牌 id。
返回布尔值。
只可以和事件连用。详情参考 `事件`。
；TODO： 以后换成链接
##参数


｜序号｜ 参数 ｜是否可选｜          描述  ｜
｜:--:｜:----:｜:------:｜:--------:｜
｜1  ｜ 卡牌 id ｜   否   ｜要判断的卡牌 id ｜


##示例
### excel-Card 表格
｜参考列｜    表头    ｜ 值 ｜
｜:----:｜:----------:｜:--:｜
｜  A   ｜     id     ｜ 150(请根据实际情况填写)   ｜
｜  B   ｜displayName ｜  测试Buff  ｜
｜…略…｜            ｜    ｜
｜  M   ｜    code    ｜ MyCmdGroup:83  ｜
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
｜  A   ｜     id     ｜  MyCmdGroup  ｜
｜  B   ｜description ｜  测试用的buff，如果受到 {cn:0} 就回复 1 点生命值  ｜
｜…略…｜            ｜    ｜
｜  M   ｜    remapCode   ｜  evt.PreAddBuff:{If:{ArgIsCard:$0},{Heal:1}}  ｜
｜…略…｜            ｜    ｜
**结果：当玩家拥有 `测试Buff` 这个Buff 的时候，每当玩家受到 id 为 83 的 buff 时都会回复 1 点 HP**
![ArgIsCardSample1](argiscard~/Images~/ARGISCARDSAMPLE1.png)
![ArgIsCardSample2](argiscard~/Images~/ARGISCARDSAMPLE2.png)
##注意
+`ArgCardHasTag` 和 `IfArgIsCard` 指令只能和事件连用！直接使用会导致意想不到的错误。

