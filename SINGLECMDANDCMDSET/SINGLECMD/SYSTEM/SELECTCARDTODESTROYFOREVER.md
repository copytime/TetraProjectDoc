
%SelectCardToDestroyForever

；2019/5/10 下午 3:30:58

[ 导航链接列表

/*Nav*/

]
# SelectCardToDestroyForever 指令

##描述
选择卡牌永久销毁，本场游戏不会再次抽到。
参数为销毁卡牌的数目。
##参数

｜序号｜ 参数 ｜是否可选｜          描述  ｜
｜:--:｜:----:｜:------:｜:--------:｜
｜1  ｜ 整数，数目 ｜   是   ｜必须销毁卡牌的数目；<br>/为空则至少选择一张｜


##示例
###示例一：
#### excel-Card 表格

｜参考列｜    表头    ｜ 值 ｜
｜:----:｜:----------:｜:--:｜
｜  A   ｜     id     ｜  150(请根据实际情况填写) ｜
｜  B   ｜displayName ｜  测试卡牌  ｜
｜…略…｜            ｜    ｜
｜  M   ｜    code    ｜  SelectCardToDestroyForever: ｜
｜…略…｜            ｜    ｜
**结果：选择 1 张卡牌永久销毁，本场游戏不会再次抽到**
![SelectCardToDestroyForeverSample1](selectcardtodestroyforever~/Images~/SELECTCARDTODESTROYFOREVERSAMPLE1.png)
![SelectCardToDestroyForeverSample2](selectcardtodestroyforever~/Images~/SELECTCARDTODESTROYFOREVERSAMPLE2.png)

###示例二：
#### excel-Card 表格

｜参考列｜    表头    ｜ 值 ｜
｜:----:｜:----------:｜:--:｜
｜  A   ｜     id     ｜  150(请根据实际情况填写) ｜
｜  B   ｜displayName ｜  测试卡牌  ｜
｜…略…｜            ｜    ｜
｜  M   ｜    code    ｜  SelectCardToDestroyForever:5 ｜
｜…略…｜            ｜    ｜
**结果：选择 5 张卡牌永久销毁，本场游戏不会再次抽到**
![SelectCardToDestroyForeverSample3](selectcardtodestroyforever~/Images~/SELECTCARDTODESTROYFOREVERSAMPLE3.png)
