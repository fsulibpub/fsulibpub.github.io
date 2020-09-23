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
      <br/><br/><a href="">Copyright and Editorial Consult</a>
    </td>
    <td>
      <img class="logo" src="{{ site.baseurl }}/assets/images/logos/network2.png" height="95px" width="95px"/>
      <br/><br/><a href="">Hosting and Tech Support</a>
    </td>
    <td>
      <img class="logo" src="{{ site.baseurl }}/assets/images/logos/OpenAccess.png"/>
      <br/><br/><a href="">Open Access</a>
    </td>
    <td>
      <img class="logo" src="{{ site.baseurl }}/assets/images/logos/bookIcon-01.png" height="95px" width="95px"/>
      <br/><br/><a href="">Indexing and Preservation</a>
    </td>
    <td>
      <img class="logo" src="{{ site.baseurl }}/assets/images/logos/DHweb.png" height="95px" width="95px"/>
      <br/><br/><a href="">Digital Scholarship</a>
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





