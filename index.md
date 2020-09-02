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
      <img class="logo" src="{{ site.baseurl }}/assets/images/logos/copyright2.png" height="70px" width="70px"/>
    </td>
    <td>
      <img class="logo" src="{{ site.baseurl }}/assets/images/logos/network2.png" height="70px" width="70px"/>
    </td>
    <td>
      <img class="logo" src="{{ site.baseurl }}/assets/images/logos/OpenAccess.png"/>
    </td>
    <td>
      <img class="logo" src="{{ site.baseurl }}/assets/images/logos/bookIcon.png" height="70px" width="70px"/>
    </td>
    <td>
      <img class="logo" src="{{ site.baseurl }}/assets/images/logos/DHweb.png" height="70px" width="70px"/>
    </td>
  </tr>
    <td>
      <a href="">Copyright and Editorial Consult</a>
    </td>
    <td>
      <a href="">Hosting and Tech Support</a>
    </td>
    <td>
      <a href="">Open Access</a>
    </td>
    <td>
      <a href="">Indexing and Preservation</a>
    </td>
    <td>
      <a href="">Digital Scholarship</a>
    </td>
  <tr>
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
    </td>
    <td>
      <img class="publications" src="{{ site.baseurl }}/assets/images/journals/journalOWL.png"/>
    </td>
    <td>
      <img class="publications" src="{{ site.baseurl }}/assets/images/projects/projILSecolo.jpg"/>
    </td>
  </tr>
  <tr>
    <td><a href="books-oer">Books and Textbooks</a></td>
    <td><a href="journals">Journals</a></td>
    <td><a href="projects">Digital Projects</a></td>
  </tr>
</table>

</div>

<hr/>

### News
<div id="news">

{% assign news_by_date = site.news | sort = "date" | reverse %}
{% for news in news_by_date %}
<h3><a href="{{ news.permalink }}">{{ news.title }}</a></h3>
{{ news.content | truncate: 200 }} <a href="{{ news.permalink }}">[read more]</a><br/>
<em>{{ news.date }}</em>
{% endfor %}
</div>





