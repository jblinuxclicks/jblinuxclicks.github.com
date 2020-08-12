---
title: Posting Source Code in Wordpress is normal
date: 2020-08-13 09:00:41.000000000 -06:00
categories:
- Devops Projects
- How-to Guides
tags:
- source code
- wordpress
header:
  teaser: /assets/ShareYourSalary-HomePage-1024x654.png
---
<p>This one is pretty much a no-brainer, but I wasn't aware of it until very recently so I thought I'd share.</p>
<p>Source code, as you've probably seen on lots of web pages, is <em>treated special</em>. And for good reasons, like readability, syntax highlighting, and to protect against the use of formatted instead of plain-text characters.</p>
<p>When I first started using my Wordpress site, I just used the &lt;code&gt; HTML tag. Which is fine. But there is no syntax highlighting, which makes reading code a little more painful. I stumbled on the <a href="http://wordpress.org/extend/plugins/syntaxhighlighter/" target="_blank">Syntax Highlighter</a> plugin which does a great job and covers many languages, but alas - I'm hosted on Wordpress.com and am restricted from adding my own plugins.</p>
<p>But wait - what's this? Wordpress.com has integrated Alex Gorbatchev's <a href="http://wordpress.org/extend/plugins/syntaxhighlighter/" target="_blank">Syntax Highlighter</a> into their instances! So all I need to do is switch from the &lt;code&gt; tag to the [sourcecode language="language"] tag! Boom, syntax highlighting in my Wordpress posts.</p>
<p>Here's a quick example of what the syntax highlighting looks like for HTML, just for kicks:</p>

**Note** The snippet below was supposed to demonstrate the WordPress syntax plugin, but this site is now hosted on Jekyll. Do not expect the result below to resemble WordPress's syntax highlighting.
{: .notice--warning}

```html
<html>
<head>
<title>This is my web page title - notice it is not highlighted by the syntax highlighter, but the tags are</title>
</head>
<body>
Awesome.
</body>
</html>
```

<p>This was a game changer for me, to the point that I've been editing my old posts to use this new tag so I can offer syntax highlighting to my readers.</p>
<p>To see a full list of the supported languages, check out the <a href="http://en.support.wordpress.com/code/posting-source-code/" target="_blank">official Wordpress post about posting source code.</a></p>
<p><strong>Update:</strong> I got burned by the WordPress auto-save feature, so this post might not have rendered correctly before. Working now!<br />
<strong>Update of the update:</strong> It wasn't the auto-save that burned me, it was the sourcecode tag. It has a nasty tendency to convert symbols into their ascii codes (like "&gt" instead of ">"). Real inconvenience, sort of ruins all of the benefits of the syntax highlighting and the like. Anyway, just be aware when you are using it.</p>
