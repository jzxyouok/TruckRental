#货车租赁系统

##v1.0版本（Date：1.24）

**功能实现及未完成的部分：**
	
- 简单实现司机注册页面和主界面
- 采用了Android Studio提供的登录模板并加以修改
- 司机注册的业务逻辑检验没有写完，并且也未能存储到数据库

<p>PS：因为这几天都忙着购置年货，还打扫家里卫生，所以做的确实比较少
****

###v1.1（Date：1.29）
**实现任务：**

对货车司机注册界面进行简单优化，并添加图片

**接下一步目标：**

- 实现主界面卡片翻转效果
- 城市所在地，单独界面处理
- 与数据库连接

最后祝大家大年初二快乐！
****
###v1.2（Date：2.1）

**实现任务：**

- 连接上数据库，并对user表单进行简单的操作和测试

#v2.0版本（2.2）

**实现任务：**

* 连接上SQLite数据库
* 写完用户的CRUD操作，并进行测试

**下一次目标：**

* 将剩下的两张表的CRUD操作写完
* 司机注册页面写出来并实现它的逻辑，即能放到数据库内
****

##v2.1（2.3）
**实现任务：**

* driver和order表单创建完成及它们的基础类（domain中）创建完成
* driver的数据库底层操作CURD完成

****
##v2.2（2.4）
**实现任务**

* order表的建立及CURD完成
* 修改以前建表时的几个错误（driver和order漏了一两个表项）
* 修改了一些命名不规范的地方和用法不统一的地方，如按钮必须都叫btn

**PS**：SQLite中本来没有boolean类型，但是拓展了这个类型，所以用这种类型存储进去，但是cursor取出来时却不能取出来，所以我把Boolean修改成了Integer，限制在0和1

****
##v2.3（2.5）

**实现任务：**

* 能从页面注册司机，司机的前后端交互基本完成

**未完成的任务：**

* 将所有需要检验属性的放到一个Tools工具类里面，并且检验错误会提示错误码