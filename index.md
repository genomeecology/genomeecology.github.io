---
---

# Welcome to our Lab!

We study the biodiversity hidden within genomes. By integrating comparative genomics, evolutionary theory, computational biology, and interpretable machine learning, we investigate how mobile DNA interacts with host genomes and how these interactions drive genome innovation, adaptation, and evolutionary diversification across the tree of life. Our work spans population-level processes through to deep evolutionary comparisons across entire kingdoms, and combines discovery-driven research with the development of user-friendly tools that empower the wider community in their genomics research.

We are based at the [Naturhistoriska Riksmuseet (Swedish Museum of Natural History)](https://www.nrm.se/engelska/in-english) in Stockholm, Sweden. Interested in joining our lab? Check out our [open positions](positions) or [drop Toby a message](contact) to learn more.

{% include section.html %}

## Highlights

{% capture text %}

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

{%
  include button.html
  link="research"
  text="See our publications"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/photo.jpg"
  link="research"
  title="Our Publications"
  text=text
%}

{% capture text %}

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

{%
  include button.html
  link="projects"
  text="Browse our projects"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/photo.jpg"
  link="projects"
  title="Our Projects"
  flip=true
  style="bare"
  text=text
%}

{% capture text %}

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

{%
  include button.html
  link="team"
  text="Meet our team"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/photo.jpg"
  link="team"
  title="Meet the Lab"
  text=text
%}
