# easy_lightnovel

一些自己顺便写的各轻小说网站的爬虫程序，Colab打开即用。

---

## ESJ_Scraper

Colab分享链接:
> https://colab.research.google.com/drive/1TkfZyeMZjq-uGVl7NKlBKJELAH_45vZ0?usp=sharing

最后更新：2024/8/19

功能：根据关键词对ESJ轻小说进行下载

待实现功能：一大堆

使用手册：见实例化部分

***使用方法：***
* Step1: 使用 **usr, pwd, domain_name, path** 实例化一个 Scraper 对象

|<font size='3'>变量名</font>|<font size='4'>含义</font>|
|---|---|
|<font size='3'>usr</font>|<font size='3'>你的用户名（ESJ是邮箱登录）</font>|
|<font size='3'>pwd</font>|<font size='3'>你的密码</font>|
|<font size='3'>domain_name</font>|<font size='3'>ESJ网站域名（https://www.esjzone.cc/）</font>|
|<font size='3'>path</font>|<font size='3'>爬取的数据保存地址</font>|

* Step2: 调用 ***scraper.set_keyword()*** 方法指定搜索关键词（不指定的情况下默认全部）

* Step3: *（可选）*调用 ***scraper.set_simplify()*** 方法来指定是否自动下载简中副本

* Step4: 调用 ***scraper.get_web_novels()*** 或者 ***scraper.get_local_novels()*** 获得小说列表

* Step5: *（可选）*调用 ***print_novels*** 查看现在爬虫获取的轻小说列表

(***scraper.get_local_novels()*** 可以指定参数 **filter** 来决定是否使用关键词对本地小说进行筛选)

* Step6: 调用 ***scraper.update_novels()*** 或 ***scraper.update_1_novel()*** 来对列表中全部小说或者指定小说进行更新

* Step7: 如果使用 **Colab** 运行此程序，可以从左侧的文件中自行下载需要的文件或者自行搭载 **Google Drive** 保存文件  
