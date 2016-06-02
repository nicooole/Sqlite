# Sqlite
关于Sqlite使用的基础，仅供大家参考。
#SQlite支持的数据类型
INTEGER  有符号整形

#创建数据库
1.使用sqlite3_open函数打开数据库  
2.使用sqlite3_exec函数执行Create Table语句  
3.使用sqlite3_close函数释放资源

#查询数据
1.使用sqlite3_prepare_v2函数预处理SQL语句  
2.使用sqlite3_bind_text函数绑定参数  
3.使用sqlite3_step函数执行SQL语句，遍历结果集  
4.使用sqlite3_column_text等函数提取字段数据   
其实严格意义上，执行查询数据之前也要打开数据库，查询完毕之后要释放资源，所以一共是六个步骤。



