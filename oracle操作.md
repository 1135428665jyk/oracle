# Oracle操作

```bash
  //增加
    ALTER TABLE tb_table ADD student_email VARCHAR(10);
  //修改
    ALTER TABLE tb_table MODIFY student_email VARCHAR(10);
  //删除
    ALTER TABLE tb_table DROP student_email;
  //删除表
    DROP TABLE tb_table;
  //删除表数据
    TRUNCATE table table;
    DELETE from table;
  //添加主键约束
    ALTER TABLE table ADD CONSTRANTS pk_studnet PRIMARY KEY(stu_num);
  //添加联合主键（创建数据表的时候创建联合主键）
    ALTER TABLE table ADD CONSTRANTS pk_studnet PRIMARY KEY(stu_num,course_id);
  //删除外键约束
    ALTER TABLE table DROP CONSTRANTS contraint_name;
  //check约束
    constraint ck_student CHECK(stu_age 6 and 30)
    ALTER TABLE table DROP CONSTRANTS ck_student_sex CHECK(stu_sex='男' or stu_sex='女');
  //创建数据库
  CREATE TABLE table_name AS SELECT column_1,column_2 FROM source_table;
```