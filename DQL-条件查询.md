###基本查询</p>
-- 1、查询指定字段 name,workno,age 返回</p>
`select name,workno,age from emp;`</p>


###-- 查询返回所有字段数据</p>
`select  id,workno,name,gender, age, idcard, workadress, entrydate from emp;`</p>

###-- 3、查询所有员工的工作地址，起别名</p>
`select workadress as '工作地址' from emp ;`</p>

###-- 4、查询没有身份证号的员工</p>
`select * from emp where idcard is null ;`</p>

###-- 5、查询有身份证号的员工</p>
`select * from emp where idcard is not null ;`</p>

###-- 查询年龄等于18或20或30的员工</p>
`select * from emp where age in(18,20,30) ;`</p>

###-- 查询姓名为两个字的员工信息</p>
`select * from emp where name like '__' ;`</p>

###-- 查询身份证号最后一位为X的员工</p>
`select * from emp where idcard like '______________X' ;`</p>
`select * from emp where idcard like '%X' ;`</p>
