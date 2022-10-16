---
layout: page
title: cat-interests
---

<section>

    <h3>INTERESTS</h3>
	<ul>
    {%for post in site.categories.INTERESTS%}
		<li><time>{{ post.date | date:"%b %y" }} - </time>
		<a href="{{ post.url | prepend: site.baseurl | replace: '//', '/' }}">
        {{ post.title }}</a>
		</li>
    {% endfor %}
    </ul>

</section>