# **🎙️软件介绍**
✏️OpenArk是一款Windows平台上的开源Ark工具. Ark是Anti-Rootkit（对抗恶意程序）的简写, OpenArk目标成为逆向工程师、编程人员的工具，同时也能为那些希望**清理恶意软件**的用户服务。
![屏幕截图 2024-07-19 180652](https://github.com/user-attachments/assets/528da66b-9e34-4c99-a815-af46453613cf)
![屏幕截图 2024-07-19 182207](https://github.com/user-attachments/assets/5c693cda-8a41-4e0c-b91b-7543f1319930)


## **废话不多说,这里贴出下载链接**
🔗https://github.com/BlackINT3/OpenArk/releases
以及SoftCnKiller的下载链接
🔗https://blog.csdn.net/hfhbutn/article/details/104799162


# **教程**📝
就拿我最近让我头疼的例子来说吧

前几天想把**搜狗输入法**给换掉,最近不知道抽什么风一直弹广告(火绒还屏蔽不了的那种),就想用**Geek**将他删掉,没想到"彻底删除后"还给我留了个根(在TIM界面中Ctrl+Shift切换输入法还是会有他的输入法窗口),于是我拿出**OpenArk**和**SoftCnKiller的锁屏广告定位**来彻底清理他(如果出现以上现象,可以试试这种方法)

**由于在删除之后编写的此教程,所以图示没有多少**
先用**SoftCnKiller的锁屏广告定位**来获取**窗口句柄**(SoftCnKiller中还有一个**弹窗定位.exe**,这个是需要用鼠标来锁定窗口,而输入法的窗口会在你使用**弹窗定位**时消失,但**锁屏广告定位**是用键盘来定位的,所以不必担心输入法窗口消失的情况)

![屏幕截图 2024-07-19 180854](https://github.com/user-attachments/assets/4aa1c979-057c-4af8-bf6b-34e602748d17)

记住**窗口句柄**后,来到OpenArk,找到**内核**,**GUI管理**,在下方搜索框中输入刚刚获得的句柄(默认过滤设置为**所有**,**正则**
搜索后会出现**SougouTSF.ime**和**SougouPY.ime**文件,之后右击,选择**转到进程**,然后右击高亮的进程,选择**查看模块**

![(3EMV729D8Q2~GA%YG%LR{M](https://github.com/user-attachments/assets/490cf8cb-495d-4a89-bcd6-2d07f0ae8889)

进去查找一番就能看到这两个文件,之后再右击,选择**卸载模块**,卸载后搜狗输入法的窗口就不会弹在TIM上了(卸载后TIM可能会报错,退出重新登陆即可)

总之这是一款功能强大的软件,能做到的也不止这些(但目前我只是用来查找及分析恶意软件)

**再贴一次下载链接**
🔗https://github.com/BlackINT3/OpenArk/releases
以及SoftCnKiller的下载链接
🔗https://blog.csdn.net/hfhbutn/article/details/104799162


