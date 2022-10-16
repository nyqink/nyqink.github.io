---
layout: page
title: cat-investing
---

<section>

    <h3>INVESTING</h3>
	<ul>
    {%for post in site.categories.INVESTING%}
		<li><time>{{ post.date | date:"%b %y" }} - </time>
		<a href="{{ post.url | prepend: site.baseurl | replace: '//', '/' }}">
        {{ post.title }}</a>
		</li>
    {% endfor %}
    </ul>

</section>