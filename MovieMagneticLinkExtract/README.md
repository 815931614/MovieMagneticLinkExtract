#### 项目简介

​	MovieMagneticLinkExtract是一个基于scrapy的电影信息爬取程序。

#### 支持

- 数据来源：

  - https://www.bugutv.net/14565.html
  - https://www.yinfans.me/

- 存储：

  mysql，MongoDB，redis

- 支持增量爬虫，数据更新

  - 增量爬虫实现方式：redis_redis
  - 数据更新
    - reids_redis只能对url去重，同一个电影在不同的网站上都存在，并且不同网站的url地址不一致、电影名称也存在添字少字，所以无法根据url、电影名称判断电影的重复性
    - 但是电影数据来源网站中都会有该电影的豆瓣链接，所以可以根据豆瓣链接进行校验重复



