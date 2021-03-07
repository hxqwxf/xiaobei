# 小北同学每天自动健康打卡
## 说明
* **若未完全显示图片,请转到有道云笔记查看中[有道云笔记](http://note.youdao.com/noteshare?id=c4a1719fd3414ffb8c54eaef69ed020a&sub=WEB0553bbccc8c451fcf9c90a36edd911a5)**
* 该代码可直接运行在本地，只需要将2.py中代码复制到本地和修改账号密码即可，每天得手动运行该程序，如需每天自动打卡，请往下阅读
* **首先准备好一个github账号,注册链接[github](https://github.com/)**
* 注册qmsg酱非必须，注册qmsg酱做签到成功提醒作用，如不需要请直接跳到Github Actions说明中,qmsg酱注册地址：https://qmsg.zendee.cn/me.html#/login
* 自行去qmsg酱官网注册账号[qmsg酱注册地址](https://qmsg.zendee.cn/me.html#/login),按照要求选择提醒机器人以及QQ号，到我的-key中得到值

## 更新说明
#### 若你fork此仓库时间比我更新时间早，请及时复制2.py中的代码到你的项目中
* 21.2.7 小北同学健康打卡提交的信息变化
* 21.3.4 签到提醒修改为qq提醒
# Github Actions说明
## 一、Fork此仓库
![](http://tu.yaohuo.me/imgs/2020/06/f059fe73afb4ef5f.png)

### 点击2.py,找到temporary中的代码，若在永川不修改，其他地区请修改。
#### 修改地址格式为**中国-重庆市-重庆市-永川区**，经纬度自行百度找到当地的经纬度填写
![](https://i.loli.net/2021/02/05/VOHl12sNArmLh8u.png)

## 二、设置账号密码

* 添加名为**XIAOBEI_USERNAME**、**XIAOBEI_PASSWORD**、**XIAOBEI_SCKEY**的变量  
* 值分别为**账号**、**密码**、**qmsg酱KEY值**（qmsg酱KEY值请看最上端说明）  
![](http://tu.yaohuo.me/imgs/2020/06/748bf9c0ca6143cd.png)
![](https://i.loli.net/2021/02/05/KrHSRJk3xYAdGy5.png)
## 三、启用Action
1. 点击**Action**，再点击**I understand my workflows, go ahead and enable them** 
![](http://tu.yaohuo.me/imgs/2020/06/34ca160c972b9927.png)
2. 点击**code**，然后往下滑动点击commint change
![步骤1](https://i.loli.net/2021/02/05/qwFmINBZp3fgiQP.png)
3. 再点击笔,在空白行随便输入东西
![步骤2](https://i.loli.net/2021/02/05/irWEo63dkwpAPyc.png)
4. 然后往下滑动点击commint change
![步骤3](https://i.loli.net/2021/02/05/gAuwbIxyaJdWPYe.png)
## 四、查看运行结果
Actions  > xioabei daka > get-points  
能看到如下图所示，表示成功  
![](https://i.loli.net/2021/02/05/iXz96WZeScOIGbE.png)

此后， 将会在每天10点多签到一次  
若有需求，可以在[.github/workflows/run.yml]中自行修改 
1
