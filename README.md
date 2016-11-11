# check_logfiles
This plugins processes a logfile (-l) and report on all time taken entries for last (-m) minutes.

The scripts are a modification from https://exchange.nagios.org/directory/Plugins/Web-Servers/Apache/check\_access\_log-2Epl/details

 ## check_Tomcatlogfile.pl:
 Processes a tomcat logfile with pattern "%a %t %H %p %U %s %S %D %I %b".

 Example: check_tomcatlogfile.pl -fp "/usr/tomcat/apache-tomcat-6.0.29/logs" -pl "tomcat_access_" -sl ".log" -r "/newResource/index.html" -w 2000 -c 5000 -m 5