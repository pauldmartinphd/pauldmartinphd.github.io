I am Chief Scientist at **Harbor Experts, Inc.** and a part-time Lecturer in the Department of Computer Science at **Johns Hopkins University**, where I teach courses on computer and network security, applied cryptography, and programming. I hold B.S., M.S.E., and Ph.D. degrees in computer science from Johns Hopkins.

My work spans secure system architecture, embedded-device security, and large-scale source-code analysis. Recent projects range from automated firmware-vulnerability detection to control-flow-integrity profiling hardware for embedded CPUs. I am a named inventor on six U.S. patents and have served on the program committee for the IEEE Symposium on Security and Privacy.

In my spare time, I restore vintage hardware, design open-source tools, and mentor students on hands-on security projects. A full curriculum vitae is available on the sidebar.

---

## Latest notes

{% if site.posts == empty %}
*No posts yet.*  
{% else %}
{% for post in site.posts limit:3 %}
* {{ post.date | date: "%b %d %Y" }} — **[{{ post.title }}]({{ post.url }})**
{% endfor %}
{% endif %}
