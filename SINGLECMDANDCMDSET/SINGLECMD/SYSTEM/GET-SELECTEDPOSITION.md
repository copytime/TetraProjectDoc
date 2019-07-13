
%get_selectedPosition

；2019/5/10 下午 1:05:54

[ 导航链接列表

/*Nav*/

]
# get_selectedPosition 指令

##描述
获取玩家选择的位置。
返回值为三维向量。
##参数

<1.2>无参数

##示例
#### excel-Card 表格

｜参考列｜    表头    ｜ 值 ｜
｜:----:｜:----------:｜:--:｜
｜  A   ｜     id     ｜  150(请根据实际情况填写) ｜
｜  B   ｜displayName ｜  测试卡牌  ｜
｜…略…｜            ｜    ｜
｜  M   ｜    code    ｜  CreateEnemy:1,{get_selectedPosition:} ｜
｜…略…｜            ｜    ｜

**结果：在选定位置生成角色 id 为 1 的敌人**

<br/>
> *技巧：* 使用 `变量语法糖` 可增加代码易读性，详情可参考 `变量语法糖 $`。

；TODO: 以后改为链接
