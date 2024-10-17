---
layout: default
title: Trimming Circles
description: A mental scrapyard for raw ideas.
---
> "The ultimate sense-enhancing device is a searching mind."

Leo here.
Most recently going by `futurisold`.
I see patterns in data.
Life's one big puzzle.
Science bug bit me young.
Made me curious.
Always asking why.
That curiosity?
It's my fuel.
Pushes me to excel.
No half measures.
Dropped out of uni.
Started from scratch.
Just me and a computer.
Always has been.
Grew up with mIRC, DC++, torrents in Eastern Europe.
I've seen things teenage me shouldn't have.
That mindset stuck.

{{ content }}

<br>

{% assign posts = site.posts %}
{%- if posts.size > 0 -%}
<ul class="post-list">
    {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
    {%- assign margin_left = -40 -%}
    {%- assign margin_top = -7 -%}
    {%- for post in posts -%}
        <h3>
          <a class="post-link" style="margin-left: {{ margin_left }}px;" href="{{ post.url | relative_url }}"> {{ post.title | escape }} </a>
        </h3>
        <span class="post-meta"
              style="margin-top: {{ margin_top }}px; display: block; margin-left: {{ margin_left }}px;">{{ post.date | date: date_format }}
        </span>
    {%- endfor -%}
</ul>
{%- endif -%}

