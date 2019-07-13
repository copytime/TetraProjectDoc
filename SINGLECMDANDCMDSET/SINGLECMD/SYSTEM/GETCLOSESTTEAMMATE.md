
%GetClosestTeammate

；2019/5/10 下午 2:57:18

[ 导航链接列表

/*Nav*/

]
# GetClosestTeammate 指令

##描述
获得最近的队友。
返回值为角色(Character类)。
##参数

<1.2>无参数
##示例
### excel-Card 表格
｜参考列｜    表头    ｜ 值 ｜
｜:----:｜:----------:｜:--:｜
｜  A   ｜     id     ｜  150(请根据实际情况填写) ｜
｜  B   ｜displayName ｜  测试卡牌  ｜
｜…略…｜            ｜    ｜
｜J｜       aimTypeCode     ｜  SingleOnly  ｜
｜…略…｜            ｜    ｜
｜  M   ｜    code    ｜  ShowEffect:6,{GetClosestTeammate:} ｜
｜…略…｜            ｜    ｜

**结果：在所选目标的最近的队友显示 id 为 6 的特效**

##注意
+ `GetClosestTeammate` 指令没法对着环境（Env）使用，因为环境没有队友。
