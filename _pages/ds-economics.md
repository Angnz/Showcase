---
permalink: /ds-economics/
layout: page
title: Data Science in Economics
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
<hr>

# Data science Posts 
<ul>
    {% for post in site.posts %}
      {% if post.categories contains 'datasc' %}
        <li><a href="{{ site.baseurl }}{{ post.url }}">{{ post.date | date: "%Y, %b %d"  }} - {{ post.title }}</a></li>
      {% endif %}
    {% endfor %}
</ul>