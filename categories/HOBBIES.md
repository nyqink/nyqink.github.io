---
layout: page
title: HOBBIES
---

<section>

    <h3>HOBBIES</h3>
	<ul>
    {%for post in site.categories.HOBBIES%}
		<li><time>{{ post.date | date:"%b %y" }} - </time>
		<a href="{{ post.url | prepend: site.baseurl | replace: '//', '/' }}">
        {{ post.title }}</a>
		</li>
    {% endfor %}
    </ul>

</section>