---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

title: Home
layout: default

---

{% include mobilebayicon.html %}

# WE ARE MOBILE BAY DSA

{% include poem.html %}

{% include socials.html %}

If you live in Mobile or Baldwin County, you can [join national DSA](https://www.dsausa.org/) and have your chapter assigned to Mobile Bay. Whether you decide to join or not, we recommend coming to our [public interest meetings](./calendar) to talk with members and hear more about our goals, principles, and projects. If you live elsewhere and have [checked that there isn't a chapter nearby](https://www.dsausa.org/chapters/), that's fine too --- you can still join DSA as an at-large member and participate in [national DSA projects](https://www.dsausa.org/get-involved/), or even [organize a new chapter](https://www.dsausa.org/chapters/start-a-chapter/) local to your own region!

<br />

## UPCOMING EVENTS

{% for post in site.categories.events reversed %}
{% if post.eventtype == "dsa future" %}
{% include eventcard.html url=post.url time=post.time place=post.place title=post.title description=post.description %}
{% endif %}
{% endfor %}