# fantasy-fa-bidding
# Send fantasy football free agent bid offers to comissioner Bowman

import smtplib
 
server = smtplib.SMTP('smtp.gmail.com', 587)
server.starttls() #make sure you leave this it protects the password
server.login("officialfantasyemail@gmail.com", "Fantasy2017")
 
msg = "Work!" #this would be the user input I was just making sure it worked
server.sendmail("officialfantasyemail@gmail.com", "BOWMANSEMAIL@gmail.com", msg) #The bowmanemail is whatever email we send it to
server.quit()
