# Introduction #

Here are the steps to make the config.inc.php file manually.sometimes it may happen that the last step of the automated installation step may be in error(i.e: Error in creating the config file).this is because your web server has blocked file access problem.This can be solved in two ways.

  1. your root directory should be given write access (e.g: 644)
> 2) or manually create the config file as shown below.


# Details #

**Step 1:** open the **config.tmp.php** file in a editor which can be found in the **/install/**  directory


**Step 2:** now start replacing the tags shown as below
> ` define('DB_SERVER', "{DB_SERVER}"); `


> here replace {DB\_SERVER} with your server address eg: localhost
> > ` define('DB_SERVER', "localhost"); `


similarly replace
//database login name

`define('DB_USER', "{DB_USER}");`
//database login password

`define('DB_PASS', "{DB_PASS}");`

//database name

`define('DB_DATABASE', "{DB_DATABASE}");`

// table prefix

`define('PQPRE', "{PQPRE}");`

`define('SITENAME',"{SITENAME}");`

`define('SITETITLE',"{SITETITLE}");`

`define('SITE_LINK',"{SITE_LINK}");`


**Step 3:** once this is done save this file as **config.inc.php**  in your **root**   directory.

> eg:  `http://www.proquiz.com/config.inc.php`

**Step 4:** thats it. make sure that before doing this please run the installation procedure as usual . remember this is just an alternative for making the config file .