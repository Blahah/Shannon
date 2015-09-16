---
layout: page
title: "Download"
group: navigation
---

{% include JB/setup %} 

#### Repository

The __kallisto__ GitHub repository is [here](http://github.com/pachterlab/kallisto).

#### Releases

<table class="table">
  <thead>
    <tr>
      <th style="text-align: left">Version</th>
      <th>Date</th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>

{% for post in site.categories.releases %}
    <tr>
    	<td>Release notes: <a href="{{ site.url }}/kallisto/{{ post.url }}">{{ post.version }}</a></td>
    	<td><span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span></td>

        <td><a href="https://github.com/pachterlab/kallisto/releases/download/{{ post.version }}/kallisto_mac-{{ post.version }}.tar.gz">Mac</a></td>
        <td>{% if post.version <= 'v0.42.1' %} <a href="https://github.com/pachterlab/kallisto/releases/download/{{ post.version }}/kallisto_linux-{{ post.version }}.tar.gz">Linux</a> {% endif %} </td>
        <td><a href="https://github.com/pachterlab/kallisto/archive/{{ post.version }}.tar.gz">Source</a></td>
    </tr>
{% endfor %} 
</table>

#### Transcriptomes

Commonly used transcriptome FASTA files are available [here](http://bio.math.berkeley.edu/kallisto/transcriptomes/).

#### Licence

Kallisto is distributed under a non-commercial [license](license.html). For commercial use, please contact Terri Sale at the Office of Technology Licensing, UC Berkeley, 2150 Shattuck Avenue, Suite 510, Berkeley, CA 94720-1620, (510) 643-4219, terri.sale@berkeley.edu.
