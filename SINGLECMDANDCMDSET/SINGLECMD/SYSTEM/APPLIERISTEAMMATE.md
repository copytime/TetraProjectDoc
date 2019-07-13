
%ApplierIsTeammate

；2019/5/10 上午 8:12:34

[ 导航链接列表

/*Nav*/

]
# ApplierIsTeammate 指令

##描述
判断指令。如果施加者是队友返回真，否则返回假。
返回值为布尔值。
##参数

<1.2>无参数



##示例
#### excel-Card 表格

｜参考列｜    表头    ｜ 值 ｜
｜:----:｜:----------:｜:--:｜
｜  A   ｜     id     ｜  150(请根据实际情况填写) ｜
｜  B   ｜displayName ｜  测试卡牌  ｜
｜…略…｜            ｜    ｜
｜  M   ｜    code    ｜  If:{ApplierIsTeammate:},{Heal:1},{TakeDamage:1}  ｜
｜…略…｜            ｜    ｜

**结果：如果施加者是队友，就回复 1 点 HP，否则就造成 1 点伤害**
![ApplierIsTeammateSample1](applieristeammate~/Images~/APPLIERISTEAMMATESAMPLE1.png)


##注意
+ `ApplierIsTeammate` 指令没有参数。



