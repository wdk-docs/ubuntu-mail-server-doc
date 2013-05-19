.. mail server doc documentation master file, created by
   sphinx-quickstart on Sun May 19 11:59:22 2013.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

MailServer 文档!
===========================================

Setting up an Ubuntu System as an Email Server
Introduction
目录

Setting up an Ubuntu System as an Email Server
Introduction
Mail Transfer Agent
Mail filtering
Mail Delivery Agent
Webmail
Mailing lists
Related Articles
Setting up an email server is a difficult process involving a number of different programs, each of which needs to be properly configured. The best approach is to install and configure each individual component one by one, ensuring that each one works, and gradually build your mail server.

Mail Transfer Agent
A Mail Transfer Agent (MTA) is the program which receives and sends out the email from your server, and is therefore the key part. The default MTA in Ubuntu is Postfix, but exim4 is also fully supported and in the main repository.

Postfix - this guide explains how to set up Postfix.

Mail filtering
You can add filtering in your mail chain, mainly in order to detect spam and viruses.

PostfixAmavisNew - this guide explains how to integrate amavisd-new with Postfix.

PostfixGreylisting - this guide explains how to install Postgrey to implement greylisting

EximClamAV - this guide explains how to integrate anti-virus with the Exim mail server

Mail Delivery Agent
In order to allow you or others to download email from other locations, you need to setup an IMAP or POP3 server. Again, there are many of these, with different advantages and disadvantages. All the servers presented here can be found in the Ubuntu main repository, which means that it receives security updates when necessary.

Dovecot - this guide explains how to set up Dovecot as a mail server. Dovecot is a good mail server which is simple to setup.

Courier - this guide explains how to set up Courier as a mail server. Courier is also quite simple to use and can be used with external database for managing virtual users. It is widely used.

MailServerCourierSpamAssassin - this guide provides an example of a complete mail server using Courier MTA and SpamAssassin.

Cyrus - this guide explains how to set up Cyrus as a mail server. Cyrus is of those MDA the most complicated server. Neverthless, it is the more scalable and a widely used server. It only supports virtual users. Warning: Cyrus has been dropped from main. It is in universe on dapper and edgy and thus doesn't necessarily receive security updates.

Webmail
Webmail permits you and your email users to view their email via their webbrowser from anywhere in the world. You'll need to have setup a MTA, a MDA and a webserver (see the Apache page) for these to work.

Squirrelmail - this guide explains how to set up Squirrelmail webmail.

OpenWebMail - this guide explains how to set up the OpenWebMail application.

Mailing lists
You can add to your mail server a mailing-list system to deliver mails to a large number of people, let someone else manage subscription, manage people who are posting, moderate messages.

Mailman - this guide explains howto setup a mailman installation on Postfix and Exim.

Related Articles
