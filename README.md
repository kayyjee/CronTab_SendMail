# CronTab_SendMail


Summary

We wrote a shell script that will prompt the user to enter a date and time. 
The date and time will be appended to the crontab in proper format. At the 
date specified by the user, a cronjob will be activated which will send 
an email to a user provided address and will be able to support text and graphic 
attachments. The path of the attachment is also specified by the user.  

Pre-steps:
	
	In order for the email to be able to send a graphic attachment, we needed to install mutt. 







Pseudo Code.
1.	Take User input for Date / Time.
a.	Take User input for month(s).
b.	Take User input for day (weekday or day of month).
c.	Take User input for hour of the day.
d.	Take User input for minutes of the hour.
2.	Take User input for Email data.
a.	Take User input for subject
b.	Take User input for body of the email.
c.	Ask user if they want an attachment.
i.	IF yes: Take User input for the path of the file to be attached.
3.	Make dir: /tmp/mailKJ.
4.	Create file mycron in /mailKJ.
5.	Create line in mycron with Email data in mutt format.
6.	Change permissions for mycron to allow execution.
7.	Append mycron to crontab with user input for Date / Time.
8.	Assign crontab file to crontab scheduler. 
