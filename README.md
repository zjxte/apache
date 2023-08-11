# apache

Heading 2 1- Go to "C:\Apache24\conf" then edit the 'httpd.conf' file and enable & edit the following lines:

Listen *:80
(OPTIONAL) LoadModule rewrite_module modules/mod_rewrite.so 
ServerName www.example.com:80 (--to) ServerName localhost:80
AllowOverride None (--to) AllowOverride All

Heading 2 2- Go to "C:\Apache24\bin" (copy the path), and open CMD as administrator.
---------------------------------------------(Commands)-------------------------------------------------------
cd C:\Apache24\bin
httpd.exe -t  ----(to check the syntax, if doesn't work, need to install Microsoft Visual C++ Redistributables)
httpd.exe -k install ----(To install the service)
httpd.exe -k start -----(To start the service) 
---------------------------------------------------------------------------------------------------------------------------
Heading 2 3- If you want to edit the output, go to "C:\Apache24\htdocs" and edit the 'index.html' file.
