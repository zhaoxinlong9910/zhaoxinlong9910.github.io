---
title: Oracle序列创建
date: 2022-08-09 09:16:07
tags:
---
# --创建序列
create sequence SEQ_MTG_USER_INFO
increment by 1
start with 1
nomaxvalue
nocycle
nocache;

# --检验序列是否创建成功(tableName代表对应表的表名)
{% codeblock %}
select SEQ_MTG_USER_INFO.nextval from dual;
{% endcodeblock %}


![](legendOracle.png)