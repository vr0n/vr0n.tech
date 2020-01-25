---
layout: default
---

# $ cat about.txt
{:id="about"}

I am a researcher and hobbyist interested in everything. My focus right now is on computers and cyber security. You can check out some of the work I've done on this very site.

# $ cat contact.txt
{:id="contact"}

<ul>
<li>mail: vstech@protonmail.ch</li>

<li>twitter: @tau_over_two</li>
</ul>

# $ cat projects.txt
{:id="projects"}

<ul>
{% for project in site.categories.projects %}
<li><a href="{{ project.link }}">{{ project.title }}</a> - {{ project.description }}</li>
{% endfor %}
</ul>

# $ cat tools.txt
{:id="tools"}

<ul>
{% for tool in site.categories.tools %}
<li><a href="{{ tool.link }}">{{ tool.title }}</a> - {{ tool.description }}</li>
{% endfor %}
</ul>

# $ cat talks.txt
{:id="talks"}

<ul>
<li>I give talks sometimes... I will post the slides here or the recordings if that ever happens.</li>
</ul>

# $ cat posts.txt
{:id="posts"}

<ul>
{% for post in site.categories.posts %}

{% if post.en %}
{% endif %}

{% endfor %}
</ul>

# $ cat articles.txt
{:id="articles"}

<ul>
{% for post in site.categories.articles %}

{% if post.en %}
{% endif %}

{% endfor %}
</ul>
