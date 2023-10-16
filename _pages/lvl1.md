---
permalink: /lvl1/
layout: page
title: "LVL1: MONKEY"
---
<style>
    body {
        font-family: Arial, sans-serif;
        background-color: #1F4172;
        margin: 2em;
        padding: 1em;
    }
    
    .site-header, .footer-heading{ /*site-header is the Webpage Banner and  text*/
        Color: #132043;
        font-family: Arial, sans-serif;
        background-color: #363062;
        color:#F99417;
        border-top:0px;
        border-bottom: 0px;
        
    }
    
    .site-title, .site-title:visited {
        color: #F99417;
    }
    
    .site-title:hover {
        text-decoration: none;
    }
    
    .site-nav .page-link{
        font-family: 'Courier New', Courier, monospace;
        color: #F99417;
        line-height: 1.5;
    }
    
    a {
        color: #FDF0F0;
    }
    
    a:visited {
        color: #00FF00;
    }
    
    .page-content{
        font-family: 'Courier New', Courier, monospace;
        color: #FDF0F0;
        line-height: 1.5;
        overflow-x: auto;
    }

     pre, code {
      background-color: transparent;
      color: black;
      font-family: 'Courier New', monospace;
      }
</style>

I want to show here my Posts iof coding lvl 1

POSTS try 1
<hr>

 {% for post in site.posts %}
  <article>
    <h2>
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
    </h2>
    <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
    {{ post.content }}
  </article>
{% endfor %}

POSTS try 2
<hr>
<p></p>
This is my review of {{post.lvl1}}.


POSTS try 3
<hr>

{%- assign posts = site.posts | where_exp: 'post', 'post.film' -%}

{%- for post in posts -%}
    Title: <a href="{{post.url |relative_url}}">{{post.title}} / {{post.lvl1}}</a><br>
{%- endfor -%}