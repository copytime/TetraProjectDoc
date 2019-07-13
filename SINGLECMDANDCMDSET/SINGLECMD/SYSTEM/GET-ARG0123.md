
%get_arg0，get_arg1，get_arg2 和 get_arg3

；2019/5/10 上午 11:22:56
[ 导航链接列表

/*Nav*/

]
# get_arg[0,1,2,3] 指令
获取事件传递的第[0,1,2,3]个参数。
返回值与传递进来的参数一致。
只可以和事件连用。详情参考 `事件`。
；TODO： 以后换成链接
##描述
加法运算。返回参数一浮点数与参数二浮点数的和。返回值为整数。
##参数

<1.2>无参数

##示例
### excel-Card 表格
｜参考列｜    表头    ｜ 值 ｜
｜:----:｜:----------:｜:--:｜
｜  A   ｜     id     ｜ 150(请根据实际情况填写)   ｜
｜  B   ｜displayName ｜  测试Buff  ｜
｜…略…｜            ｜    ｜
｜  M   ｜    code    ｜ MyCmdGroup:2   ｜
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
｜  B   ｜description ｜  测试用的buff，如果在受到 buff 时 buff 数目超过{0}就回复 1 点生命值  ｜
｜…略…｜            ｜    ｜
｜  M   ｜    remapCode   ｜  evt.PreAddBuff:{If:{>:{BuffCount:{get_arg0:}},$0},{Heal:1}}  ｜
｜…略…｜            ｜    ｜
**结果：当玩家拥有 `测试Buff` 这个Buff 的时候，每当玩家受到 buff 且 buff 数目大于 2 时都会回复 1 点 HP**
![get-argSample1](get-arg0123~/Images~/GET-ARGSAMPLE1.png)
![get-argSample2](get-arg0123~/Images~/GET-ARGSAMPLE2.png)
<br/>
> *技巧：* 使用 `变量语法糖` 可增加代码易读性，详情可参考 `变量语法糖 $`。
；TODO: 以后改为链接

##注意
+`get_arg[0,1,2,3]` 指令只能和事件连用！
