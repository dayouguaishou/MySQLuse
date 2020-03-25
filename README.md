基于Python3的对MySQL的简易查询模块
==================================================  
1.导入pymysql库  
1.1 Linux  
`sudo pip3 install pymysql`  
1.2 Windows  
`pip3 install pymysql`  

2.导入SimplifyuseMySQL  
```Python  
import SimplifyuseMySQL  
```  

3.cnf.ini 文件内容  
[db]  
db_host = 192.168.137.137  
db_port = 3306  
db_user = root  
db_pass = root@123  
db_name = test  

函数名称：cnfdb(filename = "cnf.ini")  
----
说明：从filename文件中获取mysql连接参数  
返回：dictionary（字典）-cnfg_dict{}  

函数名称：select_MYSQL(SQL)  
----
说明：查询数据库  
返回：数据集（元组）-datas() 或输出错误信息  

函数名称：select_datas_column(datas,num = 0)  
----
说明：查询数据集某一列（num）num>=0  
返回：数据列（list）-list[]  

函数名称：execute_to_mysql(SQLS)  
----
说明：执行SQL语句  
返回：无 或输出错误信息  


20200318 for Python3 by Wei.Wei
--------------------------------------------------
