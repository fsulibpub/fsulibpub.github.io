---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: Florida State Open Publishing
layout: default
---

### Our Mission

{% include mission.liquid %}

[Read more](/about)

<hr/>

### Services
<div id="services">
<table>
  <tr>
    <td>
      <img class="logo" src="{{ site.baseurl }}/assets/images/logos/copyright2.png" height="95px" width="95px"/>
      <br/><br/><p><strong>Copyright and Editorial Consult</strong></p>
      <p>We offer consultations and training on publication contracts, the use of copyrighted material in scholarly publications, and the ownership and licensing of research outputs.</p>
    </td>
    <td>
      <img class="logo" src="{{ site.baseurl }}/assets/images/logos/network2.png" height="95px" width="95px"/>
      <br/><br/><p><strong>Hosting and Tech Support</strong></p>
      <p>We host and provide technical support for publishing platforms including <a href="https://pkp.sfu.ca/ojs/" title="Public Knowledge Project homepage for Open Journal Systems">Open Journal Systems</a>, <a href="https://manifold.lib.fsu.edu/" title="Florida State Open Publishing hosted Manifold instance">Manifold</a>, and FSU's institutional repository, <a href="http://diginole.lib.fsu.edu/repository" title="Florida State University's Digital Research Repository">DigiNole</a>.</p>
    </td>
    <td>
      <img class="logo" src="{{ site.baseurl }}/assets/images/logos/OpenAccess.png"/>
      <br/><br/><p><strong>Open Access</strong></p>
      <p>We work with researchers to increase the dissemination and impact of various products of original research, including data, and provide in-depth analysis and training on the platforms, tools, and policies through which open access is evolving.</p>
    </td>
    <td>
      <img class="logo" src="{{ site.baseurl }}/assets/images/logos/bookIcon-01.png" height="95px" width="95px"/>
      <br/><br/><p><strong>Indexing and Preservation</strong></p>
      <p>We increase the discoverability of research outputs and educational resources and utilize digital preservation tools to ensure long-term access to scholarly content.</p>
    </td>
    <td>
      <img class="logo" src="{{ site.baseurl }}/assets/images/logos/DHweb.png" height="95px" width="95px"/>
      <br/><br/><p><strong>Digital Scholarship</strong></p>
      <p>We provide consultations on the use of digital tools for GIS mapping, virtual reality, text analysis, and data visualization in all stages of the research cycle.</p>
    </td>
  </tr>
</table>
</div>

<hr/>

### Publications
<div id="publications">

<table>
  <tr>
    <td>
      <img class="publications" src="{{ site.baseurl }}/assets/images/books-oer/bookSVP.jpg"/>
      <br/><br/><a href="books-oer">Books and Textbooks</a>
    </td>
    <td>
      <img class="publications" src="{{ site.baseurl }}/assets/images/journals/journalOWL.png"/>
      <br/><br/><a href="journals">Journals</a>
    </td>
    <td>
      <img class="publications" src="{{ site.baseurl }}/assets/images/projects/projILSecolo.jpg"/>
      <br/><br/><a href="projects">Digital Projects</a>
    </td>
  </tr>
</table>

</div>

<hr/>

### News
<div id="news">

{% assign news_by_date = site.news | sort = "date" | reverse %}
{% for news in news_by_date %}
<h3><a href="{{ site.baseurl }}{{ news.permalink }}">{{ news.title }}</a></h3>
{{ news.content | truncate: 200 }} <a href="{{ news.permalink }}">[read more]</a><br/>
<em>{{ news.date }}</em>
{% endfor %}
</div>





