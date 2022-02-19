---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
# Greetings, fellow nerd!
If you happened to bump into this site, seems like you also enjoy hacking,
burning electronics for fun, making and playing games and occasionally, shed a
nostalgic tear about some retro goodness.

_Stay awhile and read..._

## Making a game for the Nintendo Entertainment System
{% for page in site.nesdev %}
{{forloop.index}}. [{{page.title}}]({{page.url}})
{% endfor %}
