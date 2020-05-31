## oracle 常用命令

### SQL*plus命令

````sql
--设置行宽
--默认值为80
set linesize 160;  
-- 设置每页显示个数
--默认值为14
set pagesize 160; 
-- 设置数字显示格式
-- 9代表数字，0代表精确小数部分 $代表前缀 S显示正负 ，用于方便统计位数
set numformat S$999,999.00 
-- 查询SQL plus的命令清单
--实现所有的SQL plus命令，通过help [option] 查询相应的命令使用方式
help index 
--查询视图和表结构
--显示表结构 
describe/desc table_name 
--将查询内容保存到文件中
spool path/fileName;    spool C:/sql.txt
sql...			       select * from emp;
spool off			   spool off;
-- 将最近的sql命令保存到文件中
save fileName;
-- 将sql脚本放入缓存区中
get fileName;
--  执行一个sql脚本文件 start 和 @都可以
start fileName
-- 格式化查询结果 
-- col col_name option value
-- option [clear、format、heading、on/off ]
col name format $999,99.00
col name heading 姓名
-- TTITLE 和 BTITLE 设置表显示的头标题和尾标题
-- TTITLE  option[on|off] titleText
TTITLE 客户信息表  TTITLE off

````



### sql 基础



