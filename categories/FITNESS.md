---
layout: page
title: FITNESS
---

<section>

    <h3>FITNESS</h3>
	<ul>
    {%for post in site.categories.FITNESS%}
		<li><time>{{ post.date | date:"%b %y" }} - </time>
		<a href="{{ post.url | prepend: site.baseurl | replace: '//', '/' }}">
        {{ post.title }}</a>
		</li>
    {% endfor %}
    </ul>

</section>