I build trustworthy computing systems—from bare-metal firmware to cloud-scale analytics.  

Today I serve as **Chief Scientist at Harbor Experts**, leading embedded-security R & D and supervising a multilingual team that has performed **100 + source-code reviews** in C/C++, Go, Java, Python, Swift, Kotlin, JavaScript, TypeScript and other languages. I also provide **expert-witness testimony** in high-stakes technology matters, performing analysis and translating evidence for judges and juries.
At **Johns Hopkins University** I lecture on computer & network security, applied cryptography, hardware systems and software development.

Selected projects
---------------

* **Firmware IQ** – automated engine that unpacks embedded-device firmware and runs 100 + static checks to surface vulnerabilities including through cross-reference to NIST National Vulnerability Database.  
* **CPU-side control-flow monitor** – CPU add-on that enforces control-flow integrity on IoT-class CPUs.  
* **Smart-grid anomaly dashboard** – real-time traffic-visualisation platform now sold commercially as part of SecureSmart MSS.

Impact & outreach
-----------------

* Author of peer-reviewed papers on embedded security, multifactor authentication, and large-scale audit analysis.  
* Six U.S. patents; program-committee member for the **IEEE Symposium on Security & Privacy**.  
* **Whitepapers** on best practices for source-code review, differential comparison, and code quality analysis.  

When not teaching or writing code, I restore vintage hardware, curate retro-computing archives, and mentor emerging engineers on hands-on security and technical projects.

[Download CV (PDF)](/assets/PaulMartin-CV.pdf)

---

## Latest notes

{% if site.posts == empty %}
*No posts yet.*  
{% else %}
{% for post in site.posts limit:3 %}
* {{ post.date | date: "%b %d %Y" }} — **[{{ post.title }}]({{ post.url }})**
{% endfor %}
{% endif %}
