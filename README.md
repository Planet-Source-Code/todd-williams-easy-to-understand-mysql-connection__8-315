<div align="center">

## Easy To Understand MySQL Connection


</div>

### Description

This is to teach you how to connect to your mysql database and select a table. I have made it very clean and added comments to help you understand the process.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Todd Williams](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/todd-williams.md)
**Level**          |Beginner
**User Rating**    |4.8 (58 globes from 12 users)
**Compatibility**  |PHP 3\.0, PHP 4\.0
**Category**       |[Databases](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/databases__8-5.md)
**World**          |[PHP](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/php.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/todd-williams-easy-to-understand-mysql-connection__8-315/archive/master.zip)

### API Declarations

OPEN SOURCE, but Credit would be nice. :)


### Source Code

```
<?php
$server    = ""; //ie: mysql.server.net
$username   = ""; //ie: jonnhy
$password   = ""; //ie: password101
$databasename = ""; //ie: jonnydata
$tablename  = ""; //ie: emails
$connection = mysql_connect("$server","$username","$password");
  if(!$connection)// are we not connected?
  {
  echo "Couldn't make a connection!!!";
  exit; //exits the script
  }
  $db = mysql_select_db("$databasename",$connection);
  if(!$db) //was the database not found?
  {
  echo "The database disapeared!";
  mysql_close($connection); //closes connection
  exit; // exits the code
}
echo "If you can see this you are connected to your database and your table is selected.";
```

