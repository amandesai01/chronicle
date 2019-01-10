# Chronicle - A JDBC LOGIN PROJECT Along with DASHBOARD.
This is a NetBeans Project using `mysql-connector-java-8.0.13` .
It is a simple JDBC Project with login-logout system and Dashboard.<br>
* You can Register with "registerhere.java".
* Login with "MainSc.java".
* Dashboard is displayed by "dashboard.java"
* Add a new post with "postadder.java".

***For synchronising user among all frames, id is retrived at the time of login and is circulated through object.***
<br><br>
**MySql Database looks like this :-**
__Database__: Users
Table1: usersone (Used to save login credentials and other data.)
Coloumn:
+----+---------------+----------+----------+------------+
| ID | username      | passkey  | fname    | lname      |
+----+---------------+----------+----------+------------+

Table2: posts(Used to save post data along with its username):
Coloumn:
+----+---------------+----------------------------+--------------------------------------------------+
| id | username      | title                      | postdata                                         |
+----+---------------+----------------------------+--------------------------------------------------+

Table3: insertions
(Used to get total no of posts and last insert id. Last post's id is sent to row 1 and can b retrived whenever required by using query - 'select lstins from  insertions where id =1')
Coloumn:
+------+--------+
| id   | lstins |
+------+--------+
|    1 |    17  |
+------+--------+
