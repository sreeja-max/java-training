# java-training
SQL*Plus: Release 18.0.0.0.0 - Production on Mon Apr 26 15:38:02 2021
Version 18.4.0.0.0

Copyright (c) 1982, 2018, Oracle.  All rights reserved.

Enter user-name: conn / as sysdba
Enter password:

Connected to:
Oracle Database 18c Express Edition Release 18.0.0.0.0 - Production
Version 18.4.0.0.0

SQL> alter session set"_oracle_script"=true;

Session altered.


SQL> create user dxctesting identified by sreeja;

User created.

SQL> conn/ as sysdba
Connected.
SQL> grant create session to dxctesting;

Grant succeeded.



SQL> create table stocks
  2  (
  3  name varchar(50),
  4  id int,
  5  batchno int,
  6  symbol varchar(45)
  7  );

Table created.

SQL> create table sales
  2  (
  3  name varchar(50),
  4  id int,
  5  batchno int,
  6  symbol varchar(45)
  7  );

Table created.

SQL> select sysdate from dual;

SYSDATE
---------
26-APR-21

SQL> select to_char(sysdate,'mm-dd-yy hh:mi') from dual;

TO_CHAR(SYSDAT
--------------
04-26-21 03:57

SQL> select to_char(sysdate,'dd/mm/yy')from dual;

TO_CHAR(
--------
26/04/21

SQL> select to_char(date '2021-04-26','day') dy from dual
  2  ;

DY
---------
monday

SQL> select to_char(sysdate+10)as from dual;

TO_CHAR(SYSDATE+10
------------------
06-MAY-21
