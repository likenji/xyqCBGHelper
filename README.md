梦幻西游藏宝阁助手

Tampermonkey脚本。在梦幻西游藏宝阁（xyq.cbg.163.com）角色页面添加计算按钮，实现对角色技能和修炼等花费计算的简单功能。

2018.09.17 version0.3：通过localStorage保存输入参数。
测试环境：Chrome v68.0.3440.106；Tampermonkey v4.7。
备注：目前为止1.想要的基本功能已经实现；2.代码结构待优化，健壮性待完善；3.不同浏览器适配短时间内不会去做。
2018.09.07 version0.2：添加转换比，金价，修炼果输入框。目前只是基本功能的实现，没有结构优化和稳健性的措施。

演示

![添加的计算按钮](https://github.com/ipez/xyqCBGhelper/blob/master/image/1.png)

![新增的价格列表](https://github.com/ipez/xyqCBGhelper/blob/master/image/2.png)


#计算说明
1. 计算内容包括：师门技能，人物修炼，召唤兽控制力，辅助技能。
2. 人物修炼上限提升所需花费的计算采取以下规则：
    1)修炼上限21，修炼等级损失13；
    2)修炼上限22，修炼等级损失13、14；
    3)修炼上限23，修炼等级损失14、15、16；
    4)修炼上限24，修炼等级损失15、16、17、18；
    5)修炼上限25，修炼等级损失15、16、17、18、23。
3. 辅助技能等级超过40级才会被计算；5帮贡=1点点卡=￥0.1。
