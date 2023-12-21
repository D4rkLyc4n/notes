SQLMap Cheat Sheet:
Basic Commands:

Detect SQL Injection:

sqlmap -u <URL>

Specify Target Parameter:

sqlmap -u <URL> --data="<POST_data>" -p <parameter>

Specify Cookie for Authentication:

sqlmap -u <URL> --cookie="<COOKIE_data>"

Advanced Options:
Database Enumeration:

sqlmap -u <URL> --dbs

Retrieve Tables from Database:

sqlmap -u <URL> -D <database_name> --tables

Dump Data from Table:

sqlmap -u <URL> -D <database_name> -T <table_name> --dump

Set Level of Tests (1-5):

sqlmap -u <URL> --level=<level>

OS Shell Injection:

sqlmap -u <URL> --os-shell

Full HTTP Header Dump:

sqlmap -u <URL> --headers

Specify User-Agent:

sqlmap -u <URL> --user-agent="<User-Agent>"

Help :

sqlmap -h

Verbose Output:

sqlmap -u <URL> -v 3

Save Results to a File:

sqlmap -u <URL> --output-file=<output_file>
