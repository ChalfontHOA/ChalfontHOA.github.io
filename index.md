---
layout: home
permalink: /
title: 
image:
  feature: chalfont-ariel.png
---

<div class="tiles">
	<div class="tile">
	  <h2 class="post-title"><a href="{{ site.url }}/about">About</a></h2>
	  <p class="post-excerpt">About the Chalfont Homeowners Association</p>
	</div><!-- /.tile -->

	<div class="tile">
	  <h2 class="post-title"><a href="{{ site.url }}/documents">Documents</a></h2>
	  <p class="post-excerpt">Covenants, bylaws, community wide standards, and forms</p>
	</div><!-- /.tile -->

	<div class="tile">
	  <h2 class="post-title"><a href="{{ site.url }}/links">Links</a></h2>
	  <p class="post-excerpt">Links to helpful community information</p>
	</div><!-- /.tile -->
	
	<div class="tile">
	  <h2 class="post-title"><a href="{{ site.url }}/news">News</a></h2>
	  <p class="post-excerpt">Community news and announcements</p>
	</div><!-- /.tile -->
</div><!-- /.tiles -->

<h3>Latest News</h3>
<ul>
{% for post in site.posts limit:3 %}
  <b><li>{% if post.date %}<span>{{ post.date | date: "%B %d, %Y" }}</span> &raquo; {% endif %}<a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></li></b>
  <p>{{ post.content }}
{% endfor %}
</ul>