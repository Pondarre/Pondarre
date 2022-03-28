🐙  Welcome to the GitKraken CLI!
cd into a directory being tracked by Git and type gk graph to see what GitKraken can do.
pondarrerobin@MacBook-Pro-6 Pondarre % ssh robin@185.189.158.204
Linux groupe6 5.10.0-9-cloud-amd64 #1 SMP Debian 5.10.70-1 (2021-09-30) x86_64

The programs included with the Debian GNU/Linux system are free software;
the exact distribution terms for each program are described in the
individual files in /usr/share/doc/*/copyright.

Debian GNU/Linux comes with ABSOLUTELY NO WARRANTY, to the extent
permitted by applicable law.
Last login: Mon Mar 28 12:03:39 2022 from 185.226.32.21
robin@groupe6:~$ SHOW database
-bash: SHOW: command not found
robin@groupe6:~$ SHOW DATABASES;
-bash: SHOW: command not found
robin@groupe6:~$ sudo mysql SHOW DATABASES;
mysql  Ver 15.1 Distrib 10.5.15-MariaDB, for debian-linux-gnu (x86_64) using  EditLine wrapper
Copyright (c) 2000, 2018, Oracle, MariaDB Corporation Ab and others.

Usage: mysql [OPTIONS] [database]

Default options are read from the following files in the given order:
/etc/my.cnf /etc/mysql/my.cnf ~/.my.cnf 
The following groups are read: mysql mariadb-client client client-server client-mariadb
The following options may be given as the first argument:
--print-defaults          Print the program argument list and exit.
--no-defaults             Don't read default options from any option file.
The following specify which files/extra groups are read (specified before remaining options):
--defaults-file=#         Only read default options from the given file #.
--defaults-extra-file=#   Read this file after the global files are read.
--defaults-group-suffix=# Additionally read default groups with # appended as a suffix.

  -?, --help          Display this help and exit.
  -I, --help          Synonym for -?
  --abort-source-on-error 
                      Abort 'source filename' operations in case of errors
  --auto-rehash       Enable automatic rehashing. One doesn't need to use
                      'rehash' to get table and field completion, but startup
                      and reconnecting may take a longer time. Disable with
                      --disable-auto-rehash.
                      (Defaults to on; use --skip-auto-rehash to disable.)
  -A, --no-auto-rehash 
                      No automatic rehashing. One has to use 'rehash' to get
                      table and field completion. This gives a quicker start of
                      mysql and disables rehashing on reconnect.
  --auto-vertical-output 
                      Automatically switch to vertical output mode if the
                      result is wider than the terminal width.
  -B, --batch         Don't use history file. Disable interactive behavior.
                      (Enables --silent.)
  --binary-as-hex     Print binary data as hex
  --character-sets-dir=name 
                      Directory for character set files.
  --column-type-info  Display column type information.
  -c, --comments      Preserve comments. Send comments to the server. The
                      default is --skip-comments (discard comments), enable
                      with --comments.
  -C, --compress      Use compression in server/client protocol.
  -#, --debug[=#]     This is a non-debug version. Catch this and exit.
  --debug-check       Check memory and open file usage at exit.
  -T, --debug-info    Print some debug info at exit.
  -D, --database=name Database to use.
  --default-character-set=name 
                      Set the default character set.
  --delimiter=name    Delimiter to be used.
  -e, --execute=name  Execute command and quit. (Disables --force and history
                      file.)
  -E, --vertical      Print the output of a query (rows) vertically.
  -f, --force         Continue even if we get an SQL error. Sets
                      abort-source-on-error to 0
  -G, --named-commands 
                      Enable named commands. Named commands mean this program's
                      internal commands; see mysql> help . When enabled, the
                      named commands can be used from any line of the query,
                      otherwise only from the first line, before an enter.
                      Disable with --disable-named-commands. This option is
                      disabled by default.
  -i, --ignore-spaces Ignore space after function names.
  --init-command=name SQL Command to execute when connecting to MariaDB server.
                      Will automatically be re-executed when reconnecting.
  --local-infile      Enable/disable LOAD DATA LOCAL INFILE.
  -b, --no-beep       Turn off beep on error.
  -h, --host=name     Connect to host.
  -H, --html          Produce HTML output.
  -X, --xml           Produce XML output.
  --line-numbers      Write line numbers for errors.
                      (Defaults to on; use --skip-line-numbers to disable.)
  -L, --skip-line-numbers 
                      Don't write line number for errors.
  -n, --unbuffered    Flush buffer after each query.
  --column-names      Write column names in results.
                      (Defaults to on; use --skip-column-names to disable.)
  -N, --skip-column-names 
                      Don't write column names in results.
  --sigint-ignore     Ignore SIGINT (CTRL-C).
  -o, --one-database  Ignore statements except those that occur while the
                      default database is the one named at the command line.
  --pager[=name]      Pager to use to display results. If you don't supply an
                      option, the default pager is taken from your ENV variable
                      PAGER. Valid pagers are less, more, cat [> filename],
                      etc. See interactive help (\h) also. This option does not
                      work in batch mode. Disable with --disable-pager. This
                      option is disabled by default.
  -p, --password[=name] 
                      Password to use when connecting to server. If password is
                      not given it's asked from the tty.
  -P, --port=#        Port number to use for connection or 0 for default to, in
                      order of preference, my.cnf, $MYSQL_TCP_PORT,
                      /etc/services, built-in default (3306).
  --progress-reports  Get progress reports for long running commands (like
                      ALTER TABLE)
                      (Defaults to on; use --skip-progress-reports to disable.)
  --prompt=name       Set the command line prompt to this value.
  --protocol=name     The protocol to use for connection (tcp, socket, pipe).
  -q, --quick         Don't cache result, print it row by row. This may slow
                      down the server if the output is suspended. Doesn't use
                      history file.
  -r, --raw           Write fields without conversion. Used with --batch.
  --reconnect         Reconnect if the connection is lost. Disable with
                      --disable-reconnect. This option is enabled by default.
                      (Defaults to on; use --skip-reconnect to disable.)
  -s, --silent        Be more silent. Print results with a tab as separator,
                      each row on new line.
  -S, --socket=name   The socket file to use for connection.
  --ssl               Enable SSL for connection (automatically enabled with
                      other flags).
  --ssl-ca=name       CA file in PEM format (check OpenSSL docs, implies
                      --ssl).
  --ssl-capath=name   CA directory (check OpenSSL docs, implies --ssl).
  --ssl-cert=name     X509 cert in PEM format (implies --ssl).
  --ssl-cipher=name   SSL cipher to use (implies --ssl).
  --ssl-key=name      X509 key in PEM format (implies --ssl).
  --ssl-crl=name      Certificate revocation list (implies --ssl).
  --ssl-crlpath=name  Certificate revocation list path (implies --ssl).
  --tls-version=name  TLS protocol version for secure connection.
  --ssl-verify-server-cert 
                      Verify server's "Common Name" in its cert against
                      hostname used when connecting. This option is disabled by
                      default.
  -t, --table         Output in table format.
  --tee=name          Append everything into outfile. See interactive help (\h)
                      also. Does not work in batch mode. Disable with
                      --disable-tee. This option is disabled by default.
  -u, --user=name     User for login if not current user.
  -U, --safe-updates  Only allow UPDATE and DELETE that uses keys.
  -U, --i-am-a-dummy  Synonym for option --safe-updates, -U.
  -v, --verbose       Write more. (-v -v -v gives the table output format).
  -V, --version       Output version information and exit.
  -w, --wait          Wait and retry if connection is down.
  --connect-timeout=# Number of seconds before connection timeout.
  --max-allowed-packet=# 
                      The maximum packet length to send to or receive from
                      server.
  --net-buffer-length=# 
                      The buffer size for TCP/IP and socket communication.
  --select-limit=#    Automatic limit for SELECT when using --safe-updates.
  --max-join-size=#   Automatic limit for rows in a join when using
                      --safe-updates.
  --secure-auth       Refuse client connecting to server if it uses old
                      (pre-4.1.1) protocol.
  --server-arg=name   Send embedded server this as a parameter.
  --show-warnings     Show warnings after every statement.
  --plugin-dir=name   Directory for client-side plugins.
  --default-auth=name Default authentication client-side plugin to use.
  --binary-mode       Binary mode allows certain character sequences to be
                      processed as data that would otherwise be treated with a
                      special meaning by the parser. Specifically, this switch
                      turns off parsing of all client commands except \C and
                      DELIMITER in non-interactive mode (i.e., when binary mode
                      is combined with either 1) piped input, 2) the --batch
                      mysql option, or 3) the 'source' command). Also, in
                      binary mode, occurrences of '\r\n' and ASCII '\0' are
                      preserved within strings, whereas by default, '\r\n' is
                      translated to '\n' and '\0' is disallowed in user input.
  --connect-expired-password 
                      Notify the server that this client is prepared to handle
                      expired password sandbox mode even if --batch was
                      specified.

Variables (--variable-name=value)
and boolean options {FALSE|TRUE}  Value (after reading options)
--------------------------------- ----------------------------------------
abort-source-on-error             FALSE
auto-rehash                       TRUE
auto-vertical-output              FALSE
binary-as-hex                     FALSE
character-sets-dir                (No default value)
column-type-info                  FALSE
comments                          FALSE
compress                          FALSE
debug-check                       FALSE
debug-info                        FALSE
database                          (No default value)
default-character-set             auto
delimiter                         ;
vertical                          FALSE
force                             FALSE
named-commands                    FALSE
ignore-spaces                     FALSE
init-command                      (No default value)
local-infile                      FALSE
no-beep                           FALSE
host                              (No default value)
html                              FALSE
xml                               FALSE
line-numbers                      TRUE
unbuffered                        FALSE
column-names                      TRUE
sigint-ignore                     FALSE
port                              0
progress-reports                  TRUE
prompt                            \N [\d]> 
protocol                          
quick                             FALSE
raw                               FALSE
reconnect                         TRUE
socket                            /run/mysqld/mysqld.sock
ssl                               FALSE
ssl-ca                            (No default value)
ssl-capath                        (No default value)
ssl-cert                          (No default value)
ssl-cipher                        (No default value)
ssl-key                           (No default value)
ssl-crl                           (No default value)
ssl-crlpath                       (No default value)
tls-version                       (No default value)
ssl-verify-server-cert            FALSE
table                             FALSE
user                              (No default value)
safe-updates                      FALSE
i-am-a-dummy                      FALSE
connect-timeout                   0
max-allowed-packet                16777216
net-buffer-length                 16384
select-limit                      1000
max-join-size                     1000000
secure-auth                       FALSE
show-warnings                     FALSE
plugin-dir                        (No default value)
default-auth                      (No default value)
binary-mode                       FALSE
connect-expired-password          FALSE
robin@groupe6:~$ sudo SHOW DATABASE;
sudo: SHOW: command not found
robin@groupe6:~$ sudo mysql
Welcome to the MariaDB monitor.  Commands end with ; or \g.
Your MariaDB connection id is 30
Server version: 10.5.15-MariaDB-0+deb11u1 Debian 11

Copyright (c) 2000, 2018, Oracle, MariaDB Corporation Ab and others.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

MariaDB [(none)]> SHOW DATABASES;
+--------------------+
| Database           |
+--------------------+
| PERFORMER          |
| information_schema |
| mysql              |
| performance_schema |
| phpmyadmin         |
+--------------------+
5 rows in set (0.006 sec)

MariaDB [(none)]> ssh PERFORMER
    -> ;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MariaDB server version for the right syntax to use near 'ssh PERFORMER' at line 1
MariaDB [(none)]> mysql -h osr-mysql.unistra.fr -u <robin> -p <PERFORMER>    -> ;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MariaDB server version for the right syntax to use near 'mysql -h osr-mysql.unistra.fr -u <robin> -p <PERFORMER>' at line 1
MariaDB [(none)]> mysql -h osr-mysql.unistra.fr -u <robin> -p <PERFORMER>;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MariaDB server version for the right syntax to use near 'mysql -h osr-mysql.unistra.fr -u <robin> -p <PERFORMER>' at line 1
MariaDB [(none)]> mysql -u <robin> -p <PERFORMER>;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MariaDB server version for the right syntax to use near 'mysql -u <robin> -p <PERFORMER>' at line 1
MariaDB [(none)]> exit
Bye
robin@groupe6:~$ mysql -h osr-mysql.unistra.fr -u <robin> -p <PERFORMER>;
-bash: syntax error near unexpected token `;'
robin@groupe6:~$ mysql -u <robin> -p <PERFORMER>;
-bash: syntax error near unexpected token `;'
robin@groupe6:~$ mysql -h osr-mysql.unistra.fr -u <loginBDD> -p <nom_base>;
-bash: syntax error near unexpected token `;'
robin@groupe6:~$ sqlcmd [ /E ] /S servername\PERFORMER;  
-bash: sqlcmd: command not found
robin@groupe6:~$ mysql -h localhost -u root;
ERROR 1698 (28000): Access denied for user 'root'@'localhost'
robin@groupe6:~$ mysql -h robin -u root;
ERROR 2005 (HY000): Unknown MySQL server host 'robin' (-5)
robin@groupe6:~$ mysql -h PERFORMER -u root;
ERROR 2005 (HY000): Unknown MySQL server host 'PERFORMER' (-5)
robin@groupe6:~$ con = mysqli_connect('PERFORMER','robin','rorobibi');
-bash: syntax error near unexpected token `('
robin@groupe6:~$ con = mysqli_connect 'PERFORMER','robin','rorobibi';
-bash: con: command not found
robin@groupe6:~$ mysql -h localhost -u robin -p PERFORMER;
Enter password: 
Reading table information for completion of table and column names
You can turn off this feature to get a quicker startup with -A

Welcome to the MariaDB monitor.  Commands end with ; or \g.
Your MariaDB connection id is 32
Server version: 10.5.15-MariaDB-0+deb11u1 Debian 11

Copyright (c) 2000, 2018, Oracle, MariaDB Corporation Ab and others.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

MariaDB [PERFORMER]> SHOW DATABASE
    -> ;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MariaDB server version for the right syntax to use near 'DATABASE' at line 1
MariaDB [PERFORMER]> SHOW DATABASE;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MariaDB server version for the right syntax to use near 'DATABASE' at line 1
MariaDB [PERFORMER]> CREATE USER 'nico'@'localhost' IDENTIFIED BY 'nico';
Query OK, 0 rows affected (0.005 sec)

MariaDB [PERFORMER]> SHOW GRANTS FOR 'nico'@'host';
ERROR 1141 (42000): There is no such grant defined for user 'nico' on host 'host'
MariaDB [PERFORMER]> SHOW GRANTS FOR 'robin'@'host';
ERROR 1141 (42000): There is no such grant defined for user 'robin' on host 'host'
MariaDB [PERFORMER]> GRANT ALL PRIVILEGES ON *.* TO 'superadmin'@'localhost';
ERROR 1045 (28000): Access denied for user 'robin'@'localhost' (using password: YES)
MariaDB [PERFORMER]> GRANT ALL PRIVILEGES ON *.* TO 'superadmin'@'localhost';
ERROR 1045 (28000): Access denied for user 'robin'@'localhost' (using password: YES)
MariaDB [PERFORMER]> GRANT ALL PRIVILEGES ON *.* TO 'robin'@'localhost';
ERROR 1045 (28000): Access denied for user 'robin'@'localhost' (using password: YES)
MariaDB [PERFORMER]> exit
Bye
robin@groupe6:~$ sudo GRANT ALL PRIVILEGES ON *.* TO 'robin'@'localhost';
sudo: GRANT: command not found
robin@groupe6:~$ sudo mysql GRANT ALL PRIVILEGES ON *.* TO 'robin'@'localhost';
mysql  Ver 15.1 Distrib 10.5.15-MariaDB, for debian-linux-gnu (x86_64) using  EditLine wrapper
Copyright (c) 2000, 2018, Oracle, MariaDB Corporation Ab and others.

Usage: mysql [OPTIONS] [database]

Default options are read from the following files in the given order:
/etc/my.cnf /etc/mysql/my.cnf ~/.my.cnf 
The following groups are read: mysql mariadb-client client client-server client-mariadb
The following options may be given as the first argument:
--print-defaults          Print the program argument list and exit.
--no-defaults             Don't read default options from any option file.
The following specify which files/extra groups are read (specified before remaining options):
--defaults-file=#         Only read default options from the given file #.
--defaults-extra-file=#   Read this file after the global files are read.
--defaults-group-suffix=# Additionally read default groups with # appended as a suffix.

  -?, --help          Display this help and exit.
  -I, --help          Synonym for -?
  --abort-source-on-error 
                      Abort 'source filename' operations in case of errors
  --auto-rehash       Enable automatic rehashing. One doesn't need to use
                      'rehash' to get table and field completion, but startup
                      and reconnecting may take a longer time. Disable with
                      --disable-auto-rehash.
                      (Defaults to on; use --skip-auto-rehash to disable.)
  -A, --no-auto-rehash 
                      No automatic rehashing. One has to use 'rehash' to get
                      table and field completion. This gives a quicker start of
                      mysql and disables rehashing on reconnect.
  --auto-vertical-output 
                      Automatically switch to vertical output mode if the
                      result is wider than the terminal width.
  -B, --batch         Don't use history file. Disable interactive behavior.
                      (Enables --silent.)
  --binary-as-hex     Print binary data as hex
  --character-sets-dir=name 
                      Directory for character set files.
  --column-type-info  Display column type information.
  -c, --comments      Preserve comments. Send comments to the server. The
                      default is --skip-comments (discard comments), enable
                      with --comments.
  -C, --compress      Use compression in server/client protocol.
  -#, --debug[=#]     This is a non-debug version. Catch this and exit.
  --debug-check       Check memory and open file usage at exit.
  -T, --debug-info    Print some debug info at exit.
  -D, --database=name Database to use.
  --default-character-set=name 
                      Set the default character set.
  --delimiter=name    Delimiter to be used.
  -e, --execute=name  Execute command and quit. (Disables --force and history
                      file.)
  -E, --vertical      Print the output of a query (rows) vertically.
  -f, --force         Continue even if we get an SQL error. Sets
                      abort-source-on-error to 0
  -G, --named-commands 
                      Enable named commands. Named commands mean this program's
                      internal commands; see mysql> help . When enabled, the
                      named commands can be used from any line of the query,
                      otherwise only from the first line, before an enter.
                      Disable with --disable-named-commands. This option is
                      disabled by default.
  -i, --ignore-spaces Ignore space after function names.
  --init-command=name SQL Command to execute when connecting to MariaDB server.
                      Will automatically be re-executed when reconnecting.
  --local-infile      Enable/disable LOAD DATA LOCAL INFILE.
  -b, --no-beep       Turn off beep on error.
  -h, --host=name     Connect to host.
  -H, --html          Produce HTML output.
  -X, --xml           Produce XML output.
  --line-numbers      Write line numbers for errors.
                      (Defaults to on; use --skip-line-numbers to disable.)
  -L, --skip-line-numbers 
                      Don't write line number for errors.
  -n, --unbuffered    Flush buffer after each query.
  --column-names      Write column names in results.
                      (Defaults to on; use --skip-column-names to disable.)
  -N, --skip-column-names 
                      Don't write column names in results.
  --sigint-ignore     Ignore SIGINT (CTRL-C).
  -o, --one-database  Ignore statements except those that occur while the
                      default database is the one named at the command line.
  --pager[=name]      Pager to use to display results. If you don't supply an
                      option, the default pager is taken from your ENV variable
                      PAGER. Valid pagers are less, more, cat [> filename],
                      etc. See interactive help (\h) also. This option does not
                      work in batch mode. Disable with --disable-pager. This
                      option is disabled by default.
  -p, --password[=name] 
                      Password to use when connecting to server. If password is
                      not given it's asked from the tty.
  -P, --port=#        Port number to use for connection or 0 for default to, in
                      order of preference, my.cnf, $MYSQL_TCP_PORT,
                      /etc/services, built-in default (3306).
  --progress-reports  Get progress reports for long running commands (like
                      ALTER TABLE)
                      (Defaults to on; use --skip-progress-reports to disable.)
  --prompt=name       Set the command line prompt to this value.
  --protocol=name     The protocol to use for connection (tcp, socket, pipe).
  -q, --quick         Don't cache result, print it row by row. This may slow
                      down the server if the output is suspended. Doesn't use
                      history file.
  -r, --raw           Write fields without conversion. Used with --batch.
  --reconnect         Reconnect if the connection is lost. Disable with
                      --disable-reconnect. This option is enabled by default.
                      (Defaults to on; use --skip-reconnect to disable.)
  -s, --silent        Be more silent. Print results with a tab as separator,
                      each row on new line.
  -S, --socket=name   The socket file to use for connection.
  --ssl               Enable SSL for connection (automatically enabled with
                      other flags).
  --ssl-ca=name       CA file in PEM format (check OpenSSL docs, implies
                      --ssl).
  --ssl-capath=name   CA directory (check OpenSSL docs, implies --ssl).
  --ssl-cert=name     X509 cert in PEM format (implies --ssl).
  --ssl-cipher=name   SSL cipher to use (implies --ssl).
  --ssl-key=name      X509 key in PEM format (implies --ssl).
  --ssl-crl=name      Certificate revocation list (implies --ssl).
  --ssl-crlpath=name  Certificate revocation list path (implies --ssl).
  --tls-version=name  TLS protocol version for secure connection.
  --ssl-verify-server-cert 
                      Verify server's "Common Name" in its cert against
                      hostname used when connecting. This option is disabled by
                      default.
  -t, --table         Output in table format.
  --tee=name          Append everything into outfile. See interactive help (\h)
                      also. Does not work in batch mode. Disable with
                      --disable-tee. This option is disabled by default.
  -u, --user=name     User for login if not current user.
  -U, --safe-updates  Only allow UPDATE and DELETE that uses keys.
  -U, --i-am-a-dummy  Synonym for option --safe-updates, -U.
  -v, --verbose       Write more. (-v -v -v gives the table output format).
  -V, --version       Output version information and exit.
  -w, --wait          Wait and retry if connection is down.
  --connect-timeout=# Number of seconds before connection timeout.
  --max-allowed-packet=# 
                      The maximum packet length to send to or receive from
                      server.
  --net-buffer-length=# 
                      The buffer size for TCP/IP and socket communication.
  --select-limit=#    Automatic limit for SELECT when using --safe-updates.
  --max-join-size=#   Automatic limit for rows in a join when using
                      --safe-updates.
  --secure-auth       Refuse client connecting to server if it uses old
                      (pre-4.1.1) protocol.
  --server-arg=name   Send embedded server this as a parameter.
  --show-warnings     Show warnings after every statement.
  --plugin-dir=name   Directory for client-side plugins.
  --default-auth=name Default authentication client-side plugin to use.
  --binary-mode       Binary mode allows certain character sequences to be
                      processed as data that would otherwise be treated with a
                      special meaning by the parser. Specifically, this switch
                      turns off parsing of all client commands except \C and
                      DELIMITER in non-interactive mode (i.e., when binary mode
                      is combined with either 1) piped input, 2) the --batch
                      mysql option, or 3) the 'source' command). Also, in
                      binary mode, occurrences of '\r\n' and ASCII '\0' are
                      preserved within strings, whereas by default, '\r\n' is
                      translated to '\n' and '\0' is disallowed in user input.
  --connect-expired-password 
                      Notify the server that this client is prepared to handle
                      expired password sandbox mode even if --batch was
                      specified.

Variables (--variable-name=value)
and boolean options {FALSE|TRUE}  Value (after reading options)
--------------------------------- ----------------------------------------
abort-source-on-error             FALSE
auto-rehash                       TRUE
auto-vertical-output              FALSE
binary-as-hex                     FALSE
character-sets-dir                (No default value)
column-type-info                  FALSE
comments                          FALSE
compress                          FALSE
debug-check                       FALSE
debug-info                        FALSE
database                          (No default value)
default-character-set             auto
delimiter                         ;
vertical                          FALSE
force                             FALSE
named-commands                    FALSE
ignore-spaces                     FALSE
init-command                      (No default value)
local-infile                      FALSE
no-beep                           FALSE
host                              (No default value)
html                              FALSE
xml                               FALSE
line-numbers                      TRUE
unbuffered                        FALSE
column-names                      TRUE
sigint-ignore                     FALSE
port                              0
progress-reports                  TRUE
prompt                            \N [\d]> 
protocol                          
quick                             FALSE
raw                               FALSE
reconnect                         TRUE
socket                            /run/mysqld/mysqld.sock
ssl                               FALSE
ssl-ca                            (No default value)
ssl-capath                        (No default value)
ssl-cert                          (No default value)
ssl-cipher                        (No default value)
ssl-key                           (No default value)
ssl-crl                           (No default value)
ssl-crlpath                       (No default value)
tls-version                       (No default value)
ssl-verify-server-cert            FALSE
table                             FALSE
user                              (No default value)
safe-updates                      FALSE
i-am-a-dummy                      FALSE
connect-timeout                   0
max-allowed-packet                16777216
net-buffer-length                 16384
select-limit                      1000
max-join-size                     1000000
secure-auth                       FALSE
show-warnings                     FALSE
plugin-dir                        (No default value)
default-auth                      (No default value)
binary-mode                       FALSE
connect-expired-password          FALSE
robin@groupe6:~$ mysql -h debian -u root;
ERROR 2005 (HY000): Unknown MySQL server host 'debian' (-5)
robin@groupe6:~$ mysql -h localhost -u root;
ERROR 1698 (28000): Access denied for user 'root'@'localhost'
robin@groupe6:~$ mysql -h localhost -u root;
ERROR 1698 (28000): Access denied for user 'root'@'localhost'
robin@groupe6:~$ sudo mysql
Welcome to the MariaDB monitor.  Commands end with ; or \g.
Your MariaDB connection id is 35
Server version: 10.5.15-MariaDB-0+deb11u1 Debian 11

Copyright (c) 2000, 2018, Oracle, MariaDB Corporation Ab and others.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

MariaDB [(none)]> SHOW GRANTS FOR 'robin'@'host';
ERROR 1141 (42000): There is no such grant defined for user 'robin' on host 'host'
MariaDB [(none)]> GRANT ALL PRIVILEGES ON *.* TO 'robin'@'localhost';
Query OK, 0 rows affected (0.003 sec)

MariaDB [(none)]> SHOW GRANTS FOR 'robin'@'host';
ERROR 1141 (42000): There is no such grant defined for user 'robin' on host 'host'
MariaDB [(none)]> exit
Bye
robin@groupe6:~$ mysql -h localhost -u robin -p PERFORMER;
Enter password: 
Reading table information for completion of table and column names
You can turn off this feature to get a quicker startup with -A

Welcome to the MariaDB monitor.  Commands end with ; or \g.
Your MariaDB connection id is 36
Server version: 10.5.15-MariaDB-0+deb11u1 Debian 11

Copyright (c) 2000, 2018, Oracle, MariaDB Corporation Ab and others.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

MariaDB [PERFORMER]> SHOW GRANTS FOR 'robin'@'host';
ERROR 1141 (42000): There is no such grant defined for user 'robin' on host 'host'
MariaDB [PERFORMER]> SHOW TABLES;
+---------------------+
| Tables_in_PERFORMER |
+---------------------+
| Artist              |
+---------------------+
1 row in set (0.000 sec)

MariaDB [PERFORMER]> SHOW CREATE TABLE Artist;
+--------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Table  | Create Table                                                                                                                                                                                                                                          |
+--------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Artist | CREATE TABLE `Artist` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `nom` varchar(100) NOT NULL,
  `genre` varchar(255) NOT NULL,
  `age` int(10) NOT NULL,
  `pay` varchar(100) NOT NULL,
  PRIMARY KEY (`id`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 |
+--------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
1 row in set (0.000 sec)

MariaDB [PERFORMER]> SELECT USER();
+-----------------+
| USER()          |
+-----------------+
| robin@localhost |
+-----------------+
1 row in set (0.000 sec)

MariaDB [PERFORMER]> CREATE TABLE Concert (
    -> id INT PRIMARY KEY NOT NULL
    -> nom VARCHAR(100),
    -> hqsfiuf;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MariaDB server version for the right syntax to use near 'VARCHAR(100),
hqsfiuf' at line 3
MariaDB [PERFORMER]> CREATE TABLE Concert (
    -> nom VARCHAR(100),
    -> id INT PRIMARY KEY NOT NULL,
    -> date_concert DATE,
    -> pays VARCHAR(255),
    ->     ville VARCHAR(255),
    ->     code_postal VARCHAR(5),
    ->     nombre_achat INT
    -> )
    -> ;
Query OK, 0 rows affected (0.014 sec)

MariaDB [PERFORMER]> SHOW CREATE TABLE Concert;
+---------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Table   | Create Table                                                                                                                                                                                                                                                                                                                                   |
+---------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Concert | CREATE TABLE `Concert` (
  `nom` varchar(100) DEFAULT NULL,
  `id` int(11) NOT NULL,
  `date_concert` date DEFAULT NULL,
  `pays` varchar(255) DEFAULT NULL,
  `ville` varchar(255) DEFAULT NULL,
  `code_postal` varchar(5) DEFAULT NULL,
  `nombre_achat` int(11) DEFAULT NULL,
  PRIMARY KEY (`id`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 |
+---------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
1 row in set (0.000 sec)

MariaDB [PERFORMER]> CREATE TABLE Musique (
    -> id INT PRIMARY KEY NOT NULL,
    -> nom VARCHAR(100),
    -> date_publication DATE,
    -> nom_artist VARCHAR(100),
    -> genre VARCHAR(100),
    -> temps INT );
Query OK, 0 rows affected (0.013 sec)

MariaDB [PERFORMER]> SHOW CREATE TABLE Musique;
+---------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Table   | Create Table                                                                                                                                                                                                                                                                                             |
+---------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Musique | CREATE TABLE `Musique` (
  `id` int(11) NOT NULL,
  `nom` varchar(100) DEFAULT NULL,
  `date_publication` date DEFAULT NULL,
  `nom_artist` varchar(100) DEFAULT NULL,
  `genre` varchar(100) DEFAULT NULL,
  `temps` int(11) DEFAULT NULL,
  PRIMARY KEY (`id`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 |
+---------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
1 row in set (0.000 sec)

MariaDB [PERFORMER]> RENAME TABLE Concert  TO Evénement;
Query OK, 0 rows affected (0.006 sec)

MariaDB [PERFORMER]> SHOW TABLE;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MariaDB server version for the right syntax to use near '' at line 1
MariaDB [PERFORMER]> SHOW TABLES; 
+---------------------+
| Tables_in_PERFORMER |
+---------------------+
| Artist              |
| Evénement           |
| Musique             |
+---------------------+
3 rows in set (0.000 sec)

MariaDB [PERFORMER]> CREATE TABLE Utilisateur (
    -> id INT PRIMARY KEY NOT NULL,
    -> nom VARCHAR(100),
    -> prenom VARCHAR(100),
    -> email VARCHAR(255),
    -> date_naissance DATE,
    -> pays VARCHAR(255),
    -> ville VARCHAR(255),
    -> code_postal VARCHAR(5),
    -> nombre_achat_ticket INT
    -> );
Query OK, 0 rows affected (0.013 sec)

MariaDB [PERFORMER]> SHOW TABLES;+---------------------+
| Tables_in_PERFORMER |
+---------------------+
| Artist              |
| Evénement           |
| Musique             |
| Utilisateur         |
+---------------------+
4 rows in set (0.000 sec)

MariaDB [PERFORMER]> ALTER TABLE test
    -> dqds;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MariaDB server version for the right syntax to use near '' at line 2
MariaDB [PERFORMER]> ALTER TABLE Utilisateur 
    -> ADD mot_de_passe desc [AFTER colonne];
ERROR 4161 (HY000): Unknown data type: 'desc'
MariaDB [PERFORMER]> ALTER TABLE Utilisateur  ADD mot_de_passe [AFTER colonne];
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MariaDB server version for the right syntax to use near '[AFTER colonne]' at line 1
MariaDB [PERFORMER]> ALTER TABLE test
    -> ADD nom_colonne desc [AFTER colonne];
ERROR 4161 (HY000): Unknown data type: 'desc'
MariaDB [PERFORMER]> ALTER TABLE Utilisateur
    ->  ADD mot_de_passe [AFTER colonne];
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MariaDB server version for the right syntax to use near '[AFTER colonne]' at line 2
MariaDB [PERFORMER]> ALTER TABLE Utilisateur  ADD mot_de_passe desc [id];
ERROR 4161 (HY000): Unknown data type: 'desc'
MariaDB [PERFORMER]> ALTER TABLE Utilisateur ADD mot_de_passe [AFTER colonne];
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MariaDB server version for the right syntax to use near '[AFTER colonne]' at line 1
MariaDB [PERFORMER]> ALTER TABLE Utilisateur ADD mot_de_passe;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MariaDB server version for the right syntax to use near '' at line 1
MariaDB [PERFORMER]> ALTER TABLE Utilisateur ADD [COLUMN] mot_de_passe def_col_mdp [AFTER 'id'];
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MariaDB server version for the right syntax to use near '[COLUMN] mot_de_passe def_col_mdp [AFTER 'id']' at line 1
MariaDB [PERFORMER]> ALTER TABLE Utilisateur ADD [COLUMN] mot_de_passe def_col_mdp [AFTER id];
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MariaDB server version for the right syntax to use near '[COLUMN] mot_de_passe def_col_mdp [AFTER id]' at line 1
MariaDB [PERFORMER]> ALTER TABLE Utilisateur ADD COLUMN mot_de_passe def_col_mdp [AFTER 'id'];
ERROR 4161 (HY000): Unknown data type: 'def_col_mdp'
MariaDB [PERFORMER]> ALTER TABLE Utilisateur ADD COLUMN mot_de_passe AFTER 'id';
ERROR 4161 (HY000): Unknown data type: 'AFTER'
MariaDB [PERFORMER]> ALTER TABLE Utilisateur ADD COLUMN mot_de_passe VARCHAR(255) AFTER 'id';
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MariaDB server version for the right syntax to use near ''id'' at line 1
MariaDB [PERFORMER]> ALTER TABLE Utilisateur ADD COLUMN mot_de_passe VARCHAR(255) AFTER id;
Query OK, 0 rows affected (0.006 sec)
Records: 0  Duplicates: 0  Warnings: 0
