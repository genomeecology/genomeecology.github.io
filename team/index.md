---
title: Meet the Lab
nav:
  order: 1
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Meet the Lab

We are a diverse group of researchers with expertise in genomics, evolutionary biology, and bioinformatics. Our team is united by a shared passion for understanding the mechanisms shaping genome structure, adaptation, and biodiversity across the tree of life. Learn more about our group below, and feel free to reach out if you are interested in joining our lab or collaborating on research projects!

{% include section.html %}

{% include list.html data="members" component="portrait" filter="role == 'principal-investigator'" %}
{% include list.html data="members" component="portrait" filter="role == 'postdoc' and group == 'current'" %}
{% include list.html data="members" component="portrait" filter="role == 'phd' and group == 'current'" %}
{% include list.html data="members" component="portrait" filter="role == 'master' and group == 'current'" %}
{% include list.html data="members" component="portrait" filter="role == 'undergrad' and group == 'current'" %}

{% include section.html background="images/doubleHelix.png" dark=true %}
