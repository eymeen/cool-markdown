## Yaml, jekyll (only if you're using GitHub Pages)

this is NOT for normal README  
but if you enable GitHub Pages, you can start doing stuff that feels like cheating

---

### variables (feels small, but nice)

# {{ page.title }}

> {{ page.tagline }}

---

### reusable badges (generated, not hardcoded)

{% include badge.html text="cool" %}
{% include badge.html text="works" %}
{% include badge.html text="dynamic" %}

---

### fake UI components (this is where it gets fun)

{% include card.html title="Feature" desc="this is not real UI… just markdown + jekyll" %}

{% include card.html title="Another one" desc="you can stack these like components" %}

---

### generated lists (no manual typing)

## tools

{% for tool in page.tools %}
- {{ tool }}
{% endfor %}

---

### resources (cleaner than hardcoding links)

{% for r in site.data.resources %}
- [{{ r.name }}]({{ r.url }})
{% endfor %}

---

### conditionals (tiny logic)

{% if page.title == "cool-markdown" %}
🔥 this is the main page
{% endif %}

---

### layout effect (subtle but important)

this whole page can be centered, styled, spaced  
without touching the markdown itself

---

### what this actually means

you’re basically turning markdown into:
- reusable components
- dynamic content
- something closer to a small frontend

---

if you're not using GitHub Pages → ignore this whole section
