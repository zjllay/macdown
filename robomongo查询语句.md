# robomongo查询语句
----
* 查询付费用户ID  
<pre><code>通过手机号查询用户的
db.getCollection('users').find({phone:'15826861440'})
db.getCollection('orders').find({userId:ObjectId('58c25419993085222c84b2d9'),paid:true})</pre></cede>  
* 过滤不在imgs中的图片  
<pre><code>
db.getCollection('courses').find( { bigImage: { $not: /imgs/ } })  
过滤不在imgs中的图片并将name这个字段所有数据查询出来
db.getCollection(‘courses’).find( { bigImage: { $not: /imgs/ } },{_id:0,name :1}).sort( { $natural:-1} )
</pre></code>
* mongo的查询条件
<pre><code>
[$lt : <] 
例如：（1）查询birthday日期是 
[$lte : <=]  
[$gt : >]  
[$gte : >=]
</code></pre>
$regex: ‘imgs’  模糊查询
