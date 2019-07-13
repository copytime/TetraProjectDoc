
%DestroyThisCard

；2019/5/10 上午 11:02:23
[ 导航链接列表

/*Nav*/

]
# DestroyThisCard 指令

##描述
销毁事件传递的卡牌，本场战斗不会再次抽到。
只可以和事件连用。详情参考 `事件`。
；TODO： 以后换成链接
##参数

<1.2>无参数



##示例
#### excel-Card 表格

｜参考列｜    表头    ｜ 值 ｜
｜:----:｜:----------:｜:--:｜
｜  A   ｜     id     ｜  150(请根据实际情况填写) ｜
｜  B   ｜displayName ｜  测试卡牌  ｜
｜…略…｜            ｜    ｜
｜  M   ｜    code    ｜  evt.PreUseThisCard:{user.DestroyThisCard:};TakeDamage:1  ｜
｜…略…｜            ｜    ｜

**结果：造成 1 点并销毁这张卡牌，本场战斗不会再次抽到**

<br/>
> *技巧：* 使用 `Consumable` 指令组来设定消耗品卡牌是不错的选择，不建议直接使用 `DestoryThisCard` 指令。

##注意
+`DestroyThisCard` 指令只能和事件连用！直接使用会导致意想不到的错误。

