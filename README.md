# deliverable5
## General view of the website
![](https://github.com/Kururu1992/deliverable5/blob/master/screenshot/general_view.jpg)
##Vulnerability 1: Cross Site Scripting

    The cross site scripting will do harm to integrity rather than confidentiality and availability.  
    Base on this, a hacker can exploit this vulnerability by modification and fabrication.  The 
    malicious content and code can be hiden and sent to the web site.  For users, the malicious 
    code can access the sensitive information which is stored in web browsers.  The cross site 
    scripting is a typically attack that exploit the vulnerability passive.  The users execute the 
    script they trust, however the script is sent by hackers.  
    The cross site scripting attack can violate sensitive data and information which cause tamendous 
    data loss.
    
    There are several steps to fix vulnerability: the HTML markup should be limited to be used by users, 
    web application should have machanism to filter the users' input.
    
    The URL of the website has vulnerability:
    http://demo.testfire.net/bank/login.aspx
    
    Steps taken to exploit the vulnerability:
    1. load the login page: http://demo.testfire.net/bank/login.aspx
    2. input "><script>alert(1);</script> in the Username field.
    3. enter a radom password in Password field.
    
###screenshot (CSS)
![](https://github.com/Kururu1992/deliverable5/blob/master/screenshot/xss_login.jpg)


##Vulnerability 1: SQL injection

        The SQL injection will do harm to confidentiality and integrity, since attacker can modify 
        sensitive data,unauthorized access.  Interception and modification can exploit this vulnerability.
        Attackers can read and modify data from database.  The SQL injection is an active attack, 
        attackers use mallicious injection to get sensitive data and unauthorized access, which may cause 
        tramendous business loss.  If the attacker get the administration, it will cause further loss.  
        
        There are several steps to pretend SQL injection. 
        1. Filter the sensitive character in the parameter that needed in SQL
        2. Disable the xp_cmdshell store process, delete the relative dll
        3. Filter the exception message in server.
        
        The URL of the website has vulnerability:
        http://demo.testfire.net/bank/login.aspx
        
        Steps taken to exploit the vulnerability:
        1. load the login page: http://demo.testfire.net/bank/login.aspx
        2. input ZAP' OR '1'='1' -- in Username field
        3. input ZAP' OR '1'='1' -- in Password field
        4. press login button
        
###screenshot (SQL injection)
![](https://github.com/Kururu1992/deliverable5/blob/master/screenshot/SQL_1.jpg)
![](https://github.com/Kururu1992/deliverable5/blob/master/screenshot/SQL_2.jpg)

        
