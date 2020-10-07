---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: FSU Library Publishing
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
      <br/><br/><p>Copyright and Editorial Consult</p>
      <br/><br/><p>We offer consultations and training on journal/book publication contracts, the use of copyrighted material in theses and dissertations, and understanding ownership and licensing of research outputs.</p>
    </td>
    <td>
      <img class="logo" src="{{ site.baseurl }}/assets/images/logos/network2.png" height="95px" width="95px"/>
      <br/><br/><p>Hosting and Tech Support</p>
      <br/><br/><p>We host and provide technical support for publishing platforms like Open Journal Systems, Manifold, and FSU's institutional repository DigiNole.</p>
    </td>
    <td>
      <img class="logo" src="{{ site.baseurl }}/assets/images/logos/OpenAccess.png"/>
      <br/><br/><p>Open Access</p>
      <br/></br><p>We work with researchers to increase the access and impact of various products of original research, including data and provide in-depth analysis and training on the platforms, tools, and policies through which open access is evolving.</p>
    </td>
    <td>
      <img class="logo" src="{{ site.baseurl }}/assets/images/logos/bookIcon-01.png" height="95px" width="95px"/>
      <br/><br/><p>Indexing and Preservation</p>
      <br/></br><p>We help increase the discovery of research outputs and educational resources and utilize digital preservation tools to ensure long-term access to scholarly content.</p>
    </td>
    <td>
      <img class="logo" src="{{ site.baseurl }}/assets/images/logos/DHweb.png" height="95px" width="95px"/>
      <br/><br/><p>Digital Scholarship</p>
      <br/></br><p>We provide consultation on the use of digital tools for GIS mapping, virtual reality, text analysis, and data visualization in all stages of the research cycle.</p>
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





