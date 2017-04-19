---
layout: page
title: Gallerie
permalink: /gallery/
---

Some information about you!

### More Information

A place to include any other types of information that you'd like to include about yourself.

### Contact me

[email@domain.com](mailto:email@domain.com)

{% for image in site.static_files %}
    {% if image.path contains 'images' %}
        <img src="{{ site.baseurl }}{{ image.path }}" alt="image" />
    {% endif %}
{% endfor %}
