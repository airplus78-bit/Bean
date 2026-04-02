

| Ticket ID | Alert Message | Severity | Details | Ticket status |
| :---- | :---- | :---- | :---- | :---- |
| A-2703 | SERVER-MAIL Phishing attempt possible download of malware | Medium | The user may have opened a malicious email and opened attachments or clicked links. | **Escalated** |

| Ticket comments  |
| :---- |
| The incident detected an employee opening a malicious file from a suspicious phishing email.  The attacker’s email address was unusual pattern “[76tguyhh6tgftrt7tg.su](http://76tguyhh6tgftrt7tg.su)”, name was Def Communications, and IP address was 114.114.114.114. The email contained a couple of grammatical fractures, and it had a password-protected attachment, “paradise10789”. There was a malicious file in the attachment, which was filename="bfsvc.exe". Investigating the file hash, it was a well known malicious file. In addition, the alert severity is reported as medium. However, I decided to escalate this ticket to two SOC analyst to take action seriously  |

### **Additional information**

**Known malicious file hash**: 54e6ea47eb04634d3e87fd7787e2136ccfbcc80ade34f246a12cf93bab527f6b

**Email**:  
From: Def Communications \<76tguyhh6tgftrt7tg.su\>  \<114.114.114.114\>  
Sent: Wednesday, July 20, 2022 09:30:14 AM  
To: \<hr@inergy.com\> \<176.157.125.93\>  
Subject: Re: Infrastructure Egnieer role

Dear HR at Ingergy,

I am writing to express my interest in the engineer role posted from the website.

There is attached my resume and cover letter. For privacy, the file is password protected. Use the password paradise10789 to open. 

Thank you,

Clyde West  
Attachment: filename="bfsvc.exe"