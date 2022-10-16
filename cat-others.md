---
layout: page
title: cat-others
---

<section>

    <h3>OTHERS</h3>
	<ul>
    {%for post in site.categories.OTHERS%}
		<li><time>{{ post.date | date:"%b %y" }} - </time>
		<a href="{{ post.url | prepend: site.baseurl | replace: '//', '/' }}">
        {{ post.title }}</a>
		</li>
    {% endfor %}
    </ul>

</section>