---
layout: post
title:  "Ruby Logger"
date:   '2017-10-14 03:00:00'
last_modified_at:  '2017-10-14 03:30:00'
excerpt: "How to use Ruby Logger."
categories: Technology
tags:  ruby
image:
  feature: logger-bart.png
  topPosition: -150px
  width: initial
bgContrast: dark
bgGradientOpacity: darker
syntaxHighlighter: no
---
<p>
The Logger class, as the name suggests provides Logging functionality to jot down important points that you can use to output different kind of messages.
The messages can be of different severities aka levels;
</p>
<table style="width: 100%">
	<tbody>
		<tr>
			<td>LEVEL</td>
			<td>SUMMARY</td>
		</tr>
		<tr>
			<td>UNKNOWN</td>
			<td>Unknown messages are the unexpected or random messages and they should always be logged.</td>
		</tr>
		<tr>
			<td>FATAL</td>
			<td>An error that was not handled and could lead to program crashing</td>
		</tr>
		<tr>
			<td>ERROR</td>
			<td>An error that can be handled</td>
		</tr>
		<tr>
			<td>WARN</td>
			<td>A warning</td>
		</tr>
		<tr>
			<td>INFO</td>
			<td>Generic information about the usage from the code being executed</td>
		</tr>
		<tr>
			<td>DEBUG</td>
			<td>Information that was deduced during debugging</td>
		</tr>
	</tbody>
</table>

<p>
	The order goes like;
	<b>debug < info < warn < error < fatal < unknown</b>
</p>

<p>
	They work as;
	In production mode, you can set-up your Logger to output the messages which are either INFO messages or of the WARN level.
	While in development mode, you would want to keep a tab on the program’s state and its status and therefore, you can set the Logger to the DEBUG level.
</p>

<p>The interface is normally used as follows;</p>
<div class="img img--fullContainer img--14xLeading" style="background-image: url({{ site.baseurl_posts_img }}ruby-logger-3.png); height: 9rem;"></div>

<p>
	You also have the option to set an expiration date to the Log file. For ex, I want to keep the logs only for the current month. In that case I will be proceeding as follows:
</p>
<div class="img img--fullContainer img--14xLeading" style="background-image: url({{ site.baseurl_posts_img }}ruby-logger.png); height: 9rem;"></div>

<p>And on an application level,</p>
<div class="img img--fullContainer img--14xLeading" style="background-image: url({{ site.baseurl_posts_img }}Ruby-logger-2.png); height: 22rem;"></div>

<p>
	Happy logging !<br><br>
	<i>Signing out,<br>
	Niyanta</i>
</p>