- json 格式是标准的数据交换
- 前后端开发， /api json格式来交流
- 全栈  fullstack

- restful 一切皆资源
  暴露资源
- 设计良好的URL 
  /posts  拿到所有文章
  /posts/:id   :id动态匹配
  /comments 
  /comments/:id  
  /posts/1/comments   某篇文章的所有评论


- HTTP 动词有哪些？
常用的HTTP动词有下面四个（括号里是对应的SQL命令）。

GET（SELECT）：从服务器取出资源（一项或多项）。
POST（CREATE）：在服务器新建一个资源。
PUT（UPDATE）：在服务器更新资源（客户端提供改变后的完整资源）。
DELETE（DELETE）：从服务器删除资源。
还有三个不常用的HTTP动词。

PATCH（UPDATE）：在服务器更新(更新)资源（客户端提供改变的属性，比如说某个字段+1）。
HEAD：获取资源的元数据。
OPTIONS：获取信息，关于资源的哪些属性是客户端可以改变的。


HTTP 动词
GET  查询
加一条评论  增加一个资源
POST 新增  /comments
DELETE    /posts/2
PUT/PATCH  修改  /comments/2  body  最美的不是下雨天，是与你
PUT  把全新的所有的内容， 去替换掉旧的内容
PATCH  只要传递更新的字段， 局部

- RESTFUL 考点
  认为一切皆资源，URL是唯一定位资源的符号，它有一定的设计规则
  HTTP动词是Web资源的状态转换动词

  操作     SQL方法   HTTP动词
  CREATE   CREATE   POST
  READ     SELECT   GET
  UPDATE   UPDATE   PUT/PATCH
  DELECT   DELECT   DELECT











yarn add json-server
npm run server