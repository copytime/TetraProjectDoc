
%get_user

；2019/5/10 下午 1:13:19

[ 导航链接列表

/*Nav*/

]
# get_user 指令

##描述
获得施加这个指令的角色。
##参数

<1.2>无参数



##示例
#### excel-Card 表格

｜参考列｜    表头    ｜ 值 ｜
｜:----:｜:----------:｜:--:｜
｜  A   ｜     id     ｜  150(请根据实际情况填写) ｜
｜  B   ｜displayName ｜  测试卡牌  ｜
｜…略…｜            ｜    ｜
｜  M   ｜    code    ｜  If:{tgt.IsSameTeamWith:$user},{Heal:1},{TakeDamage:1} ｜
｜…略…｜            ｜    ｜

**结果：如果目标和使用者是同一队伍就回复 1 点 HP，否则造成 1 点伤害**
![get-userSample1](get-user~/Images~/GET-USERSAMPLE1.png)
<br/>
> *技巧：* 使用 `变量语法糖` 可增加代码易读性，详情可参考 `变量语法糖 $`。

；TODO: 以后改为链接

##注意
+`get_user` 指令的返回值是角色本身(Character类)。
