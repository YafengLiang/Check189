天翼云盘签到

forked from [Wang-KH/Cloud189Checkin-Actions](https://github.com/Wang-KH/Cloud189Checkin-Actions)

天翼云盘每天签到1次，抽奖2次（可多账号）

- Fork此仓库

![](https://i.loli.net/2021/09/13/qc1Cy6mMnXa2YjO.jpg)

- ##设置用户名、密码

添加名为**USER**、**PWD**、**WWBOT**(可选)、**DINGDINGBOT**(可选)、**SCKEY**(可选)的变量
值分别为**账号**、**密码**、**企业微信群聊机器人的url地址**、**钉钉群聊机器人的url地址**(在钉钉中创建时，验证方式选关键字，填入“签到”)、**Server酱的KEY**
多账号时账号密码一行一个一一对应

USER

```
123456
12345
```

PWD

```
cdse
cver
```

![image-20210913114908691](https://i.loli.net/2021/09/13/rjJSVALXcW9lh3I.png)

钉钉设置步骤：

​	创建项目（群聊），添加机器人，点击机器人头像

![image-20210913115146113](https://i.loli.net/2021/09/13/ypZlRW5TGSP7QYU.png)

自定义关键词、复制此链接  填入Secrets中的DINGDINGBOT

![image-20210913115311718](https://i.loli.net/2021/09/13/YfEjMPDksZWJN5C.png)

- ##启用Action

1 点击**Action**，再点击**I understand my workflows, go ahead and enable them**

2 修改任意文件后提交一次

![img](https://i.loli.net/2021/09/13/AiQCEGBvVy3TeZk.png)

- ##查看运行结果

Actions > Cloud189Checkin > build
能看到如下图所示，表示成功

<img src="https://i.loli.net/2021/09/13/aHJ19iTIYhZNSVv.png" alt="img" style="zoom:100%;" />

此后，将会在每天9:01开始签到
若有需求，可以在[.github/workflows/run.yml]中自行修改

60天后会自动停止，可以收到邮件  打开邮件连接，自动提转到Actions中，打开enable开关就行

