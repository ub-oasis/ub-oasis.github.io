---
title: "Team"
layout: gridlay
sitemap: false
permalink: /team/
---

## Team

### Principal Investigator / Lab Director

<div class="section-card">
<div class="pi-card">
<img src="{{ site.baseurl }}/images/team/varun-chandola.jpg" class="pi-photo" alt="Varun Chandola" loading="lazy">
<div>
<h3 class="pi-name">Varun Chandola</h3>
<p style="font-style: italic; color: var(--text-secondary);">Associate Professor, Computer Science and Engineering &bull; School of Engineering and Applied Sciences (SEAS)</p>
<div class="pi-links">
{% if site.email %}<a href="mailto:{{ site.email }}" class="icon-link" title="Email"><i class="fa-solid fa-envelope"></i></a>{% endif %}
{% if site.links.google_scholar and site.links.google_scholar != "" %}<a href="{{ site.links.google_scholar }}" class="icon-link" title="Google Scholar"><i class="ai ai-google-scholar"></i></a>{% endif %}
{% if site.links.github and site.links.github != "" %}<a href="{{ site.links.github }}" class="icon-link" title="GitHub"><i class="fa-brands fa-github"></i></a>{% endif %}
{% if site.links.linkedin and site.links.linkedin != "" %}<a href="{{ site.links.linkedin }}" class="icon-link" title="LinkedIn"><i class="fa-brands fa-linkedin"></i></a>{% endif %}
{% if site.links.twitter and site.links.twitter != "" %}<a href="{{ site.links.twitter }}" class="icon-link" title="Twitter"><i class="fa-brands fa-x-twitter"></i></a>{% endif %}
</div>
{% if site.data.pi[0].education %}
<ul style="margin-top: var(--space-4);">
{% for education in site.data.pi[0].education %}
<li>{{ education }}</li>
{% endfor %}
</ul>
{% endif %}
</div>
</div>
</div>

{% if site.data.team_members.size > 0 %}
### Current Researchers &amp; Graduate Students

<div class="team-grid">
{% for member in site.data.team_members %}
<div class="team-card">
<img src="{{ site.baseurl }}/images/{{ member.photo }}" class="team-photo" alt="{{ member.name }}" loading="lazy">
<h4 class="team-name">{{ member.name }}</h4>
<p class="team-info">{{ member.info }}</p>
<div class="team-links">
{% if member.email %}<a href="mailto:{{ member.email }}" class="icon-link" title="Email"><i class="fa-solid fa-envelope"></i></a>{% endif %}
{% if member.cv %}<a href="{{ site.baseurl }}/{{ member.cv }}" class="icon-link" title="CV"><i class="ai ai-cv"></i></a>{% endif %}
{% if member.website %}<a href="{{ member.website }}" class="icon-link" title="Website"><i class="fa-solid fa-house"></i></a>{% endif %}
{% if member.scholar %}<a href="{{ member.scholar }}" class="icon-link" title="Google Scholar"><i class="ai ai-google-scholar"></i></a>{% endif %}
{% if member.github %}<a href="{{ member.github }}" class="icon-link" title="GitHub"><i class="fa-brands fa-github"></i></a>{% endif %}
{% if member.linkedin %}<a href="{{ member.linkedin }}" class="icon-link" title="LinkedIn"><i class="fa-brands fa-linkedin"></i></a>{% endif %}
</div>
</div>
{% endfor %}
</div>
{% endif %}

{% if site.data.alumni.size > 0 %}
### Alumni

<div class="section-card">
<table class="alumni-table">
<thead>
<tr>
<th>Name</th>
<th>Years</th>
<th>Current Position / Next Destination</th>
<th>Links</th>
</tr>
</thead>
<tbody>
{% for member in site.data.alumni %}
<tr>
<td><strong>{{ member.name }}</strong></td>
<td>{{ member.duration }}</td>
<td>{{ member.info }}</td>
<td>
<div class="team-links" style="justify-content: flex-start; margin-top: 0;">
{% if member.scholar %}<a href="{{ member.scholar }}" class="icon-link" title="Google Scholar"><i class="ai ai-google-scholar"></i></a>{% endif %}
{% if member.github %}<a href="{{ member.github }}" class="icon-link" title="GitHub"><i class="fa-brands fa-github"></i></a>{% endif %}
{% if member.linkedin %}<a href="{{ member.linkedin }}" class="icon-link" title="LinkedIn"><i class="fa-brands fa-linkedin"></i></a>{% endif %}
{% if member.cv %}<a href="{{ site.baseurl }}/{{ member.cv }}" class="icon-link" title="CV"><i class="ai ai-cv"></i></a>{% endif %}
</div>
</td>
</tr>
{% endfor %}
</tbody>
</table>
</div>
{% endif %}

### Join the Lab

<div class="callout callout-info" markdown="0">
<p>We are always looking for passionate PhD students, MS students, undergraduate researchers, and high-school students interested in Artificial Intelligence, Anomaly Detection, Advanced Cyberinfrastructure and Data Science.</p>
<p>If you are interested in joining our group, please reach out to Dr. Chandola via email at <a href="mailto:chandola@buffalo.edu">chandola@buffalo.edu</a> with your CV and a brief statement of research interests.</p>
</div>
