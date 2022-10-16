---
layout: page
title: READING
---

<section>

    <h3>READING</h3>
	<ul>
    {%for post in site.categories.READING%}
		<li><time>{{ post.date | date:"%b %y" }} - </time>
		<a href="{{ post.url | prepend: site.baseurl | replace: '//', '/' }}">
        {{ post.title }}</a>
		</li>
    {% endfor %}
    </ul>

</section>