<div align="center">

![Paul Martin headshot](/Personal Portrait.jpg){: width="160" style="border-radius:50%;"}

# Paul D. Martin

**Computer scientist · Educator · Systems builder**

</div>

I study and teach computer architecture, operating systems, and security.  
My work blends low-level engineering with a historical perspective—  
from 8-bit micros to modern cloud platforms. When I’m not lecturing at Johns Hopkins, I restore vintage hardware, design open-source tools, and write about the craft of building reliable systems.

---

## Quick links

- **Curriculum Vitae:** [PDF](/assets/PaulMartin-CV.pdf)  
- **Projects:** [see the projects page](/projects/)  
- **Publications & writing:** [Google Scholar](https://scholar.google.com/citations?user=XXXXX)  
- **Contact:** [how to reach me](/contact/)

---

## Latest notes

{% if site.posts == empty %}
*No posts yet.*  
{% else %}
{% for post in site.posts limit:3 %}
* {{ post.date | date: "%b %d %Y" }} — **[{{ post.title }}]({{ post.url }})**
{% endfor %}
{% endif %}

---

*Site generated with [Jekyll](https://jekyllrb.com/) &nbsp;·&nbsp; Source on [GitHub](https://github.com/pauldmartinphd/pauldmartinphd.github.io)*
