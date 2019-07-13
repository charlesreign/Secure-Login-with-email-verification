# Secure-Login-with-email-verification
Install xampp server and navigate into the installation directory and perfom the following


In php.ini 
[mail function] 
change to:

SMTP=smtp.gmail.com
smtp_port=587
sendmail_from = my-gmail-id@gmail.com
sendmail_path = "\"C:\xampp\sendmail\sendmail.exe\" -t"


In sendmail.ini replace to this:

[sendmail]
smtp_server=smtp.gmail.com
smtp_port=587
error_logfile=error.log
debug_logfile=debug.log
auth_username=my-gmail-id@gmail.com
auth_password=my-gmail-password
