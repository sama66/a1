a site for classical form 'dhrupad'
===================

my first attemt at Jekyll and GitHub

{% if page.img %}
    	<img class="caption__media" data-interchange="{% for img in page.img %}[/assets/img/{{img[1]}} ({{img[0]}})]{% unless forloop.last %}, {% endunless %}{% endfor %}">
{% endif %}

{% if page.img %}
	<img src="/assets/img/{{ page.img.small }}{{ prepend: site.baseurl }}" alt="{{ page.img.alt }}">
{% endif %}