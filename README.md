# spider_baike
抓取百度百科关于Python词条下1000个链接页面的数据，并输出到output.html文件。Python2.7的版本

# 爬虫调度端

## URL管理器：
管理待抓取URL集合和已抓取URL集合，防止重复抓取和循环抓取

- 添加新的URL到待爬取集合中
- 判断待添加URL是否在容器中
- 获取待爬取URL
- 判断是否还有待爬取URL
- 将URL从待爬取移动到已爬取

```
$ 实现方式：
内存：Python内存。set()
关系数据库：MySQL。urls(url, is_crawled)
缓存数据库：Redis。set()
```

## 网页下载器：
- urllib2
- requests

## 网页解析器：
- 正则表达式（模糊匹配）
- html.parser（结构化解析）
- BeautifulSoup（结构化解析）
- lxml（结构化解析）

## 一个简单的爬虫实例：
- 确定目标
- 分析目标：URL格式、数据格式、网页编码
- 编写代码
- 执行代码
