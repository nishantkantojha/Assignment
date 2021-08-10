# Simple Mail Transfer Protocol


Simple Mail Transfer Protocol (SMTP) is an acronym for Simple Mail Transfer Protocol. It is a protocol that allows you to send and receive emails. SMTP, which is a set of communication standards that enables applications to send electronic mail over the internet. It's an application that uses e-mail addresses to deliver messages to other computer users. It allows users on the same or separate computers to exchange email, and it also supports:
*	It has the capability of sending a single message to one or many recipients.
* Text, voice, video, or images can be used to send a message.
*	It can also deliver messages through networks that are not connected to the internet.

![SMTp Prptocol](https://cdn.educba.com/academy/wp-content/uploads/2019/07/smtp-protocol.png.webp)

SMTP's primary function is to establish communication rules between servers. The servers can identify themselves and announce the type of communication they are attempting. They also have a system in place to deal with mistakes like wrong email addresses. If the recipient address is incorrect, for example, the receiving server will respond with some sort of error message.  An email sent over an SMTP server is known as an SMTP email. Messages are retrieved from the receiver's side using POP (Post office protocol) or IMAP (Internet message protocol). SMTP is a protocol for sending emails from one domain to another that is not the user's domain. It's used to address difficulties like email IP blacklisting and deliverability, among others. 


##	Knowing about SMTP through a video:
What is SMTP-Simple Mail Transfer Protocol?
https://www.youtube.com/watch?v=PJo5yOtu7o8

##	Model of SMTP system 
The user agent (UA) in the SMTP paradigm is Microsoft Outlook, Netscape, Mozilla, and so forth. MTA is used to exchange messages via TCP. Because the system administrator is responsible for setting up a local MTA, the user sending the mail does not have to deal with it. The MTA keeps a small backlog of messages to plan repeat deliveries if the recipient is unavailable. The MTA distributes mail to mailboxes, and user agents can then retrieve the information.
 
There should be two components in both the SMTP client and the SMTP server: 
1.	Local MTA 
2)	User Agent (UA)         
Sender-to-receiver communication: The message is prepared and sent to the MTA by the sender's user agent. The MTA's job is to transmit mail from the sender's MTA to the receiver's MTA across the network. A client MTA is required to send emails, whereas a server MTA is required to receive emails. 

##	Working of SMTP

**	Mail Composition: A user composes an electronic mail message using a Mail User Agent to send an e-mail (MUA). A software that sends and receives mail is known as a Mail User Agent. The message is divided into two parts: the body and the header. The body of the message is the most important section, whereas the header contains information like the sender and recipient addresses. The message's subject is also included in the header. The message content is analogous to a letter, and the header is analogous to an envelope with the address of the receiver.

**	Mail Submission: After creating an email, the mail client sends it to the SMTP server through SMTP on TCP port 25.

**	Delivery of Mail: E-mail addresses include two parts: the recipient's username and the domain name. For instance, vraj@gmail.com, where "Vraj" is the recipient's username and "gmail.com" is the domain. If the recipient's email address's domain name differs from the sender's domain name, MSA will route the message to the Mail Transfer Agent (MTA). The MTA will look for the destination domain to transmit the email. To get the destination domain, it looks for the MX record in the Domain Name System. The MX record contains the recipient's domain's domain name and IP address. MTA connects to the exchange server to transmit the message after the record has been found.

**	Mail Receipt and Processing: When an incoming message is received, the exchange server sends it to the incoming server (Mail Delivery Agent), which keeps it until the user retrieves it.

**	Mail Access and Retrieval: MUA may be used to retrieve email saved in MDA (Mail User Agent). Login and password are required to access MUA.

##	SMTP Fundamentals 

SMTP stands for Simple Mail Transfer Protocol. It is a protocol that is used at the application layer. The client who wants to send the email establishes a TCP connection with the SMTP server and then transmits the message across it. The listening mode of the SMTP server is always on. The SMTP process connects to port 25 as soon as it detects a TCP connection from any client.

## SENDING EMAIL

A sequence of request and response messages are sent between the client and the server to send mail. A header and a body make up the message that is sent across. The mail header is terminated by a null line, and everything following the null line is considered the message body, which is a sequence of ASCII characters. The real information read by the receipt is included in the message body.

## RECEIVING EMAIL

On the server side, the user agent checks the mailboxes at predetermined intervals. If any information is received, the user will be notified. When the user attempts to view the mail, a list of mails with a brief description of each mail in the inbox appears. The contents of any message may be viewed on the terminal by choosing it.

## Some SMTP Commands: 
** HELO - A fully qualified domain name that identifies the client to the server and is only transmitted once per session.

** MAIL — Send a message with the fully qualified domain of the sender.

**	RCPT - Follows MAIL, identifies an addressee (usually the fully qualified name of the addressee), and uses one RCPT for each addressee if there are several addressees.

**	DATA - transmit data one line at a time.

#### Message type:
For electronic mail transfer, the Simple Mail Transfer Protocol (SMTP) is an internet standard communication protocol. SMTP is used to transmit and receive emails by mail servers and other message transfer agents.
SMTP is a push protocol that is used to transmit mail, whereas POP or IMAP (internet message access protocol) is used to retrieve mail at the receiver's end.

#### Message sequence:
Three commands/reply sequences make up an SMTP transaction: The MAIL command, also known as return-path, reverse-path, bounce address, mfrom, or envelope sender, is used to determine the return address. To establish a message recipient, use the RCPT command. This command can be repeated as many times as necessary, one for each recipient. The client who wishes to send email establishes a TCP connection with the SMTP server and then transmits the message across that connection. The SMTP server is continuously listening for connections. The SMTP process starts a connection on that port as soon as it detects a TCP connection from any client (25).
                                            
 
( https://en.wikipedia.org/wiki/File:SMTP-transfer-model.svg )

#### Type of connection:
The basic protocol for sending email via the internet is SMTP (Simple Mail Transfer Protocol). Applications like Apple Mail and Outlook utilize SMTP to upload emails to mail servers, which subsequently relay them to other mail servers.
For electronic mail transfer, the Simple Mail Transfer Protocol (SMTP) is an internet standard communication protocol. SMTP is used to transmit and receive mail messages by mail servers and other message transfer agents.

 
( https://www.mailjet.com/feature/smtp-relay/ )

#### Understanding of SMTP Protocol:
The SMTP Protocol's major goal is to provide standards for server communication. The servers introduce themselves and the type of communication that is taking place. Errors like invalid email addresses are handled by servers as well. The recipient server, for example, will respond with an error message if the recipient address is wrong.

### Advantages of SMTP Protocol
**	SMTP allows email communication between several machines in a network to be as simple as possible.

**	SMTP is built on a basic infrastructure that makes sending emails simple and rapid.

**	For outgoing email messages, SMTP provides dependability, which means that if a message is not delivered successfully, the SMTP server will try to resend the message until it is sent successfully.

** Organizations can use SMTP to manage outbound email messages if they have a dedicated server.

**	Connecting to SMTP is simple and straightforward. It has a simple installation process.

**	SMTP connections are unrestricted and can connect to any system. All we must do now is plug in the SMTP details.

**	It excludes any future development on our part.


##	Conclusion
Email is quickly becoming one of the most important online services. Most internet systems utilize SMTP to transmit messages from one user to another. SMTP is a push protocol that is used to transmit mail, whereas POP (post office protocol) or IMAP (internet message access protocol) are used to retrieve mail at the recipient's end. Sending emails and messages to individuals all around the world is made simple with SMTP. Bulk emailing is only feasible using SMTP servers, and it is one of the most cost-effective ways to send emails to a large group of individuals at once.

##	Bibliography
https://www.youtube.com/watch?v=PJo5yOtu7o8
https://www.geeksforgeeks.org/simple-mail-transfer-protocol-smtp/
https://www.educba.com/smtp-protocol/
Video: https://www.youtube.com/watch?v=PJo5yOtu7o8

## Group Members:

1. Darshini Jayrambhai Ratadiya

   **Student Id:** 139945208
   
   **Email Id:** djratadiya@myseneca.ca


2. Nishant Kant Ojha

   **Student Id:** 142488204
   
   **Email Id:** nkojha@myseneca.ca

3. Puja Girishkumar Kakani

   **Student Id:** 138344205
   
   **Email Id:**: pgkakani@myseneca.ca

