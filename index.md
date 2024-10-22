---
layout: page_lab
---

{% assign lab = "ciel" %}
{% assign teams_sorted = site.labs | where: "cat", lab | where: "subcat", "team" | sort: "title"  %}
{% assign cells_sorted = site.labs | where: "cat", lab | where: "subcat", "cell" | sort: "title"  %}

<!-- Banner -->
<section id="banner">
<div class="content" style="width: 100%;">
  <p>
    The “Cerebral Imaging and Engineering Laboratory” (CIEL) is dedicated to the development of innovative methodologies for understanding the biophysics of brain mechanisms, such as metabolism, neuronal activity and molecules transport, both in normal and pathological conditions. These developments are strongly supported by:
    <ul>
      <li>the use of high and ultra-high field MRI scanners dedicated to small animals (7T, 11.7T and 17.2T) to investigate specific brain functions with unprecedented spatio-temporal resolution and sensitivity to molecules of interest;</li>
      <li>the integration of additional technologies such as ultrasound, 2-photons microscopy, electrophysiology and histology, to better capture the complexity of the biophysical processes under investigation or to propose new tools for modulating these processes;</li>
      <li>an integrated translational approach, starting from the optimization of all methodological and technological developments on dedicated animal models before working on their transfer into a clinical setting.</li>
    </ul>
  </p>
  <p>
    Therefore, the global scientific strategy of CIEL consists in building a framework of imaging technologies that are increasing the comprehension of fundamental mechanisms underlying brain functioning, but also in producing new diagnostic and therapeutic tools in a pathological context such as brain tumor, stroke, neurodegenerative and psychiatric diseases. 
  </p>
  <p>
  Below is a list of all the <a href="#teams">teams</a> and <a href="#cells">cells</a>. A <a href="#gallery">gallery</a> of current research topics is also available.
  </p>
  <!-- <p>
  <b>Teams:</b>
  {% for team in teams_sorted %}
    {% if team.site %}
        <a href="{{team.site}}">{{team.title}}</a>
    {% else %}
        <a href="{{site.url}}{{site.baseurl}}{{team.url}}">{{team.title}}</a>
    {% endif %}
  {% endfor %}
  <br>
  <b>Cells:</b>
  {% for cell in cells_sorted %}
    {% if cell.site %}
        <a href="{{cell.site}}">{{cell.title}}</a>
    {% else %}
        <a href="{{site.url}}{{site.baseurl}}{{cell.url}}">{{cell.title}}</a>
    {% endif %}
  {% endfor %}
   </p> -->
</div>
<div class="">
  <img src="{{site.url}}{{site.baseurl}}/images/banner.png" alt="" style="
    width: 100%;
    height: auto;
    margin-bottom: 2em;
  "/>
</div>
</section>

