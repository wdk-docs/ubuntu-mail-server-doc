MailServer 文档!
===========================================

在Ubuntu系统上设置邮件服务器

介绍
-----

由于对服务器的配置需要涉及到数个不同的程序，而只有在所有程序都得到了正确的配置之后服务器才能正常工作，因此这个过程可能会显得比较困难。最好的办法就是一个接一个进行组件的安装配置操作，确保每一个都能工作,逐步地建立起您的邮件服务器。

传输代理
--------

（MTA 邮件传输代理）是一个用来接受并转发邮件的程序，它是整个服务器的关键部分。在Ubuntu中默认的邮件传输代理程序是Postfix，主软件库中的exim4也是完全支持的。

* Postfix :doc:`/postfix` - 将会指导您如何安装并设置Postfix。

过滤
--------

您可以添加过滤到您的邮件链中，主要是为了检测垃圾邮件和病毒。

* PostfixAmavisNew - this guide explains how to integrate amavisd-new with Postfix.
* PostfixGreylisting - this guide explains how to install Postgrey to implement greylisting
* EximClamAV - this guide explains how to integrate anti-virus with the Exim mail server

分发代理
--------

为了让您或者是其他人能够从其他地点下载邮件，您需要安装并设置一台IMAP或者POP3邮件服务器。此类服务器数量众多，各有优缺。在这里所提到的所有的服务器都能够在Ubuntu主软件仓库中找到，这就意味着它们能在需要时进行安全升级。

* Dovecot - this guide explains how to set up Dovecot as a mail server. Dovecot is a good mail server which is simple to setup.

* Courier - this guide explains how to set up Courier as a mail server. Courier is also quite simple to use and can be used with external database for managing virtual users. It is widely used.

* MailServerCourierSpamAssassin - this guide provides an example of a complete mail server using Courier MTA and SpamAssassin.

* Cyrus - this guide explains how to set up Cyrus as a mail server. Cyrus is of those MDA the most complicated server. Neverthless, it is the more scalable and a widely used server. It only supports virtual users. Warning: Cyrus has been dropped from main. It is in universe on dapper and edgy and thus doesn't necessarily receive security updates.

邮件前端
--------

Webmail permits you and your email users to view their email via their webbrowser from anywhere in the world. You'll need to have setup a MTA, a MDA and a webserver (see the Apache page) for these to work.

* Squirrelmail - this guide explains how to set up Squirrelmail webmail.

* OpenWebMail - this guide explains how to set up the OpenWebMail application.

邮件列表
--------

You can add to your mail server a mailing-list system to deliver mails to a large number of people, let someone else manage subscription, manage people who are posting, moderate messages.

* Mailman - this guide explains howto setup a mailman installation on Postfix and Exim.

相关文章
--------

* POP3Aggregator - this guide explains how to set up an IMAP mail server with Dovecot that will download your mail from an external POP3 server, and allow you to access the mail using any IMAP-compatible email client.
