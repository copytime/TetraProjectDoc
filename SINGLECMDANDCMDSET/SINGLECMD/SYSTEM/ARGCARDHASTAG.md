
%ArgCardHasTag



[ 导航链接列表

/*Nav*/

]
# ArgCardHasTag 指令

##描述
判断事件传递的第一个参数的卡牌是否有指定 tag。
参数为 tag 标签。
返回布尔值。
只可以和事件连用。详情参考 `事件`。
；TODO： 以后换成链接
##参数


｜序号｜ 参数 ｜是否可选｜          描述  ｜
｜:--:｜:----:｜:------:｜:--------:｜
｜1  ｜ tag 标签 ｜   否   ｜要判断的卡牌标签 ｜


##示例
### excel-Card 表格
｜参考列｜    表头    ｜ 值 ｜
｜:----:｜:----------:｜:--:｜
｜  A   ｜     id     ｜ 150(请根据实际情况填写)   ｜
｜  B   ｜displayName ｜  测试Buff  ｜
｜…略…｜            ｜    ｜
｜  M   ｜    code    ｜ MyCmdGroup:   ｜
｜…略…｜            ｜    ｜


｜参考列｜    表头    ｜ 值 ｜
｜:----:｜:----------:｜:--:｜
｜  A   ｜     id     ｜ 151(请根据实际情况填写)   ｜
｜  B   ｜displayName ｜  测试卡牌  ｜
｜…略…｜            ｜    ｜
｜  M   ｜    code    ｜ AddBuff:150   ｜
｜…略…｜            ｜    ｜
### excel-CardCommand 表格
｜参考列｜    表头    ｜ 值 ｜
｜:----:｜:----------:｜:--:｜
｜  A   ｜     id     ｜  MyCmdGroup  ｜
｜  B   ｜description ｜  测试用的buff，如果受到 Debuff 就回复 1 点生命值  ｜
｜…略…｜            ｜    ｜
｜  M   ｜    remapCode   ｜  evt.PreAddBuff:{If:{ArgCardHasTag:Debuff},{Heal:1}}  ｜
｜…略…｜            ｜    ｜
**结果：当玩家拥有 `测试Buff` 这个Buff 的时候，每当玩家受到 Debuff 时都会回复 1 点 HP**
![ArgCardHasTag](argcardhastag~/Images~/ARGCARDHASTAG.png)
![ArgCardHasTagSample2](argcardhastag~/Images~/ARGCARDHASTAGSAMPLE2.png)

##注意
+ `ArgCardHasTag` 指令只能和事件连用！



