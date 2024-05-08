---
permalink: /about/
title: "About"
author_profile: true
---

from jinja2 import Template

# Define the template
template = Template("""
## Authors

{% for author in authors %}
- Name: {{ author.name }}
    Bio: {{ author.bio }}
{% endfor %}
""")

# Define some test data
authors = [
    {"name": "Author 1", "bio": "Bio 1"},
    {"name": "Author 2", "bio": "Bio 2"},
]

# Render the template with the test data
output = template.render(authors=authors)

# Print the output
print(output)