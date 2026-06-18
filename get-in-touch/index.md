---
title: Get in Touch
nav:
  order: 6
  tooltip: Email, address, and location
---

# {% include icon.html icon="fa-regular fa-envelope" %}Get in Touch

Feel free to reach out with questions, collaborations, or just to say hi!

_Interested in joining the lab?_ Check out our [open positions](positions) or [drop Toby a message](contact) if you are interested in developing a fellowship proposal (_e.g._ DDLS, Marie Curie, EMBO, Carl Tryggers, Wenner Gren, etc.).

{%
  include button.html
  type="email"
  text="Tobias.Baril@nrm.se"
  link="tobias.baril@nrm.se"
%}
{%
  include button.html
  type="phone"
  text="(555) 867-5309"
  link="+1-555-867-5309"
%}
{%
  include button.html
  type="address"
  tooltip="Our location on Google Maps for easy navigation"
  link="https://www.google.com/maps/place/Museum+of+Natural+History/@59.3689751,18.0513031,17z/data=!4m6!3m5!1s0x465f9d06c299a63d:0xe5f99fa024a7bfd!8m2!3d59.3689751!4d18.053878!16zL20vMDZuZzd3!5m1!1e2?entry=ttu"
%}

{% include section.html %}

{% capture col1 %}

{%
  include figure.html
  image="images/highlights/NRM.jpeg"
  caption="NRM Stockholm"
%}

{% endcapture %}

{% capture col2 %}

{%
  include figure.html
  image="images/photo.jpg"
  caption="Lorem ipsum"
%}

{% endcapture %}

{% capture col3 %}

{%
  include figure.html
  image="images/photo.jpg"
  caption="Lorem ipsum"
%}

{% endcapture %}

{% include cols.html col1=col1 col2=col2 col3=col3 %}
