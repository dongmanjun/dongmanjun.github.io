# Welcome to 动漫君 Pages 
**动漫君欢迎您**  <img align="right" src="529710224727080979.gif"/>

新浪微博    [weibo](https://weibo.com/3991135975)

哔哩哔哩    [bilibili](https://space.bilibili.com/47764900)

网易云音乐  [163music](https://music.163.com/#/user/home?id=406836144)

# Name
**动漫君**


# instagram @dongmanjun
[instagram](https://www.instagram.com/dongmanjun/)

# [©动漫君](https://dongmanjun.github.io)

---
layout: null
---

<?xml version="1.0" encoding="utf-8"?>
<feed xmlns="https://dongmanjun.github.io">

 <title>{{site.title}}</title>
 <link href="{{site.url | prepend:site.baseurl}}/atom.xml" rel="self"/>
 <link href="{{site.url | prepend:site.baseurl}}/"/>
 <updated>{{site.time | date_to_xmlschema}}</updated>
 <id>{{site.url}}</id>
 <author>
   <name>{{site.author.name}}</name>
   <email>{{site.author.email}}</email>
 </author>

 {% for post in site.posts %}
 <entry>
   <title>{{post.title | xml_escape}}</title>
   <link href="{{site.url | prepend:site.baseurl}}{{post.url}}"/>
   <updated>{{post.date | date_to_xmlschema}}</updated>
   <id>{{site.url}}{{post.id}}</id>
   <content type="html">{{post.content | xml_escape}}</content>
 </entry>
 {% endfor %}

</feed>
