Title: Configure email account

# Configure email account

This document aims to present a step-by-step of the email configuration in 4biz Platform by reading (IMAP) and sending (SMTP) messages.

## Before getting started

Get the email information and configure the access permissions in the email server.

**Procedure**

1.	Access the main menu Parametrization > Email
    
    - Configure the SMTP

    |ID |Description | Example |
    |---|----------|---------|
    |10 | Organization Email Address	| company@exemple.com |
    |11 | Requires authentication | Yes |
    |12 | Email adress | your.email@gmail.com |
    |13 | Password | Your Gmail password |
    |14 | Server for sending email (SMTP) | smtp.gmail.com |
    |199| Requires TLS/SSL | Yes |
    |269| Port| 587 |


    - Configure the IMAP

    |ID | Description | Example |
    |---|-----------|---------|
    |23 | Server for receiving emails (IMAP) | imap.gmail.com |
    |24 | Email address | your.email@gmail.com |
    |25 | Password | Your Gmail password |
    |26 | Protocol (imaps, pop, etc.) | imaps |
    |27 | Port | 993 |
    |28 | Email box | inbox |
    |72 | Number of messages loaded | 10 |
    |199| Requires TLS/SSL | Yes |

	
!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2020 
	
