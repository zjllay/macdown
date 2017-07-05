# 快乐学习python  
----
* [git的使用方法](https://gist.github.com/guweigang/9848271)
* [tablib的使用1](http://blog.sina.com.cn/s/blog_6c532e550102vbuh.html)
* [python逐行读取文件的内容](http://www.cnblogs.com/sysuoyj/archive/2012/03/14/2395789.html)
* [tablib的使用2](http://blog.sina.com.cn/s/blog_6c532e550102vbuh.html)
* [将excel文件转换成json文件](http://www.cppblog.com/zdhsoft/archive/2011/08/10/152897.html)
* [pip命令](http://www.jianshu.com/p/41a9c25273b1)
* [python借鉴文档](https://zmywly8866.github.io/2015/01/07/use-python-get-csdn-blog-star-vote.html)  
* [requests借鉴文档](http://docs.python-requests.org/zh_CN/latest/user/quickstart.html)  
* [selenium](http://www.cnblogs.com/fnng/p/3160606.html)  
   [selenium安装以及使用](http://selenium-python.readthedocs.io/installation.html#introduction)  
* [Monkey日志分析详情](http://www.cnblogs.com/lynn-li/p/5989051.html)  
[monkey实例](http://www.bubufx.com/detail-1544794.html)
* [关于爬虫的实例](https://zhuanlan.zhihu.com/xlz-d)

###1、python补充包  
----  
> 
  * requests负责连接网站，处理http协议
  * BS4负责将网页变成结构化数据，方便爬取  
>  
  
###2、python抓取网页资源的多种方法 
><html><ol>
><li>最简单
><pre><code>
import urllib.request
response = urllib.request.urlopen('http://python.org/')
html = response.read()
  </code></pre>
></li><li>使用Request</li>
><pre><code>
> import urllib.request
req = urllib.request.Request('http://python.org/')
response = urllib.request.urlopen(req)
the_page = response.read()
></pre></code>
></ol>
></html>  

###3、高级python知识罗列  
 * 如何在列表，字典，集合中根据条件筛选数据
  * 实际案例  

> <html><ol><li>过滤掉列表[3,9,-1,10,20,-2...]中的负数  
> </ol></li> 
> <pre><code>
  
> </pre></code>
> <ol><li>筛选字典{'LiLei':79,'Jim':88,'lUCY':92...}中的值高于90的数 
> </ol></li>
> <pre><code>
  
>  </pre></code>
> <ol><li>筛选集合{77,89,32,20...}中能被3整除的元素
> </ol></li>
>  <pre><code>
  
> </pre></code> 
></html> 
  
###4、python+selenium
> 1、打开Firefox浏览器  
> <pre><code>
> 
> </code></pre>  