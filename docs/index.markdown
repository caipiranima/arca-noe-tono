---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

<ol>
{% for image in site.static_files %}
	{% if image.path contains 'pdf' %}
	<li>
		<a href="{{ site.baseurl }}{{ image.path }}">{{image.basename}}</a>
	</li>
	{% endif %}
{% endfor %}
</ol>