---
layout: page
title: cat-reading
---

<section>

    <h3>{{ category_name }}</h3>
	<ul>
    {%for post in site.categories.READING%}
		<li><time>{{ post.date | date:"%d %b %y" }} - </time>
		<a href="{{ post.url | prepend: site.baseurl | replace: '//', '/' }}">
        {{ post.title }}</a>
		</li>
    {% endfor %}
    </ul>
    
</section>