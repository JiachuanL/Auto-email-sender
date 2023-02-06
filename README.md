# Auto-email-sender
A script to monitor the live time currency exhange rate (CNY wo AUD) and send the rate to the receiver email if the rate under the threshold that the user set.
The function of the project:

Insert the receiver email, the expected currency exchange rate, and the monitor time interval.
The button check would check the format of your input.
The button send starts to send email to the receiver email address if the current currency exchange rate is lower than the input expected rate (threshold). 
i.e. if the monitor time is 30, it would get the live currency rate every 30 minutes and compare the live rate with your input threshold to determine whether to send the email.
The button stop kills the process created by the send button.
The button exit closes the main window.

This project includes the following packages:

1. Selenium: to access the website and get the live time data. (The live exchange rate of CNY to AUD).
2. Smtplib and email: to setup the access to sender email via SSL and send the rate to the receiver.
3. tkinter: to create a GUI to interact with the normal users.
4. threading: create thread to run the main loop.
