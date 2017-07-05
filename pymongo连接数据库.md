# pymongo连接数据库
----  
<html><ul><li>
 [macdown语法](http://xiajian.github.io/rhg-zh/zh/markdown/)  </li><li>
 [pymongo语句操作](http://www.jb51.net/article/64991.htm)  </li><li>
 [关于pymongo](http://simpleb.logphp.com/list/cHl0aG9uIHB5bW9uZ28g5Y246L29.html)</li><li>
 [pymongo语句](http://www.runoob.com/mongodb/mongodb-remove.html)  </li><li>
 [mongoDB的函数](https://docs.mongodb.com/manual/reference/method/cursor.pretty/)</li>
</html>  

* 1、用pynongo连接到10.8.8.8的allus数据库
  * (1) import pymongo用来验证pymongo安装成功
  * (2) pymongo连接数据库</p>

  ><pre><code>from pymongo import MongoClient
     
     > conn = MongoClient("mongo启动的主机IP",27017)  
     > db = conn.allus(数据库名称)  
     > print(db)  
     > （文档就是一条数据，集合就是表的意思）</code></pre>
 
 
 * (3) pymongo连接数据库的指定表  

 > <pre><code>videos_ coll(属性名) = db.get_collection('查询的表名')
 > print(videos _coll)</code></pre>
 
* 对数据库中的集合进行操作
 * 1、查询
 * (1)	查询集合中所有的元素  

 > <pre><code>for video in db.videos.find():(videos是集合：即表名)  
 >     print(video)  </code></pre>
 
 * （2）从数据库中读取5条数据到本地  

 > <pre><code>  
 >fout = open('a.json','w',encoding = 'utf-8')
 > count = 0
 >for video in db.videos.find(): 
 >    if count < 5: 
 >    		fout.write(str(video)+'\n') 
 >	  else: 
 > 			break 
 >print(video) 
 ></code></pre>  
 
 * (3)	按照条件对指定的数据进行查询
 <br>
 <html>
 	<table>
 		<ul>
 		<li></li>
 		</ul>
 	</table>
 	
	</table>
 </html>
   **nihao**
   *j*
   ~niha~
    '<hello>'
    '''ruby
    def add(a,b)
    	return a+b
    end
    '''
    