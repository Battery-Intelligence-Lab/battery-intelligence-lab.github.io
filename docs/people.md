---
layout: page
title: People
menu-order: 20
hero-image-origin: 50% 40%
---
<div class="row">
{% assign people = site.data.people -%}
{% for group in people %}
{% if group.role != 'Alumni' %}
<div class="image-grid {{group.role | downcase | replace: ' ', '-'}}">
<h3>{{group.role}}</h3>
<ul>
	{% for person in group.people %}
		<li id="{{person.name | downcase | replace: ' ', '-'}}">
			<div class="person-row">
				<div class="photo">
					<img src="{{ site.baseurl }}/img/people/{{person.image}}" alt="{{person.name}}" title="{{person.name}}{% if person.image-credit %} (image credit: {{ person.image-credit }}){% endif %}">
					<h5 class="name sm-bottom-margin">{{person.name}}{% if person.title %} <span>{{person.title}}</span>{% endif %}</h5>
				</div>
				<div class="details" >
					{% if person.bio %}<p class="sm-top-margin">{{person.bio}}</p>{% endif %}
				</div>
			</div>
		</li>
	{% endfor %}
</ul>
</div>
{% else %}
</div>
<div class="row">
	<div class="col-xs-12">
		<h5>{{group.role}}</h5>
		<ul>
		{% for person in group.people %}
			<li>{{person}}</li>
		{% endfor %}
		</ul>
	</div>
</div>
{% endif %}
{% endfor %}

---

<div class="row">
<div class="col-xs-12 col-md-10 col-lg-8 col-md-offset-1 col-lg-offset-2" markdown="1">

#### Joining the group

**Postdocs:** Postdoctoral positions will be [advertised](https://eng.ox.ac.uk/jobs/) via the department's website. 

**DPhils:** The group is always interested in high quality doctoral applicants. The key deadline you must hit is around November each year, for the following year October start; note that all _references_ also need to be submitted by the same deadline. The admissions process at Oxford is extremely competitive, and we usually only take 1-2 students per year in this group. There are, unfortunately, only a very limited number of scholarships for international students available. There are slightly more funding opportunities for [UK home students](https://www.ox.ac.uk/students/fees-funding/fees/status), although the process is still very competitive. Applicants should consider carefully whether their interests are aligned with the group, and whether they meet the department and university admissions criteria. Further details may be found at the [Department of Engineering Science website](https://www.eng.ox.ac.uk/study/postgraduate/courses/) and you can get an idea of the project topics [here](https://eng.ox.ac.uk/study/postgraduate/applications/postgraduate-projects) (click on "electrical and optoelectronics panel") - these are just for guidance, you are welcome to propose your own.

**Internships:** We are not able to host internship students.

**Enquiries:** We receive a lot of emails about intern, doctoral, and postdoc opportunities, and do not have time to reply to all of them. Speculative enquiries about postdocs and internships will usually not be answered. 

</div>
</div>
