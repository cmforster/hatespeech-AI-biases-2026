**Sciences Po Paris**

> By: Carla Forster, Tomás Quintino Gouveia, Meire Klemmer, Aparna Rajesh, Naomi Schwarz

# Executive summary
![Annotation differences Us&AMT]({{ '/assets/images/vis 2.png' | relative_url }})
![Annotation differences Us&AMT]({{ '/assets/images/vis 3.png' | relative_url }})
![Annotation differences Us&AMT]({{ '/assets/images/vis6.png' | relative_url }})

Executive summary placeholder

## Chapters
{% assign chapters = site.pages | where_exp: "p", "p.order" | sort: "order" %}
<ol>
{% for c in chapters %}
  <li><a href="{{ c.url | relative_url }}">{{ c.title }}</a></li>
{% endfor %}
</ol>
