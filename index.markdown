---
layout: home
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

    nav{

        display:none;
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
    
    .fenster{
    
        background-color: #068DA9; /* Color azul crema */
        border-radius: 5px; /* Bordes redondeados */
        box-shadow: 5px 5px 5px #E5D283;
        max-width: 960px;
        padding: 20px;
        margin-top: 1em;
        margin-bottom: 1em;
    }

    .fenster_lvl1 {
    
        background-color: #016A70; /* Color */
        border-radius: 5px; /* Bordes redondeados */
        box-shadow: 5px 5px 5px #E5D283;
        max-width: 960px;
        padding: 20px;
        margin-top: 1em;
        margin-bottom: 1em;
    }

    .fenster_lvl2 {
    
        background-color: #1B6B93; /* Color */
        border-radius: 5px; /* Bordes redondeados */
        box-shadow: 5px 5px 5px #E5D283;
        max-width: 960px;
        padding: 20px;
        margin-top: 1em;
        margin-bottom: 1em;
    }
    
    
    fenster-letters{
        color:#333;
    }
    
    .console {
        background-color: #333;
        color: #00ff00;
        padding: 10px;
        font-family: 'Courier New', monospace;
        border: 1px solid #00ff00;
        line-height: 1;
        margin: 2em;
    }
    
    li {
        line-height: 1.5em;
    }
    
    .messagebox {
        font-size: 1em;
        background-color: gray;
        color: #f0f0f0;
        padding-top: 1em;
        padding-bottom: 1em;
        padding-left: 2em;
        margin-left: 2em;
    }
    
    .messagebox::before {
        content: "\2192";
        margin-right: 10px;
    }
    
    </style>
    
# 🖖🏻 Greetings,

I'm Angelus, an intellectually challenged chimp with an alien parasite inside me. To survive, 
I must learn coding to transfer my consciousness into a tech-bio entity.
I'm determined to save myself from this cosmic invader.

I intend to use this page as a resource for learning coding, with a goal to perfect my skills in HTML, CSS, JavaScript, PHP, Python, SPSS, Java, Ruby, SQL and R. This page will serve as my gateway to mastering a wide range of programming languages and technologies.

<div class="console">
    Difficulty and logical challenge rating
    <br>
    <br>
    <ul>
        <li>lvl 1: Monkey</li>
        <li>lvl 2: Bob</li>
        <li>lvl 3: Prometheus</li>
        <li>lvl 4: Spock</li>
    </ul>
    </div>


# Projects
## Runnnig Projects

<div class="fenster_lvl1">

    <p class="fenster-letters"><h2>Lvl 1: Simple Background Color</h2>
    <hr><br> A simple Clock in html, JS, and CSS.<br>It contains:</p>

    <div class="console">
 <ul>
        <li>JavaScript</li>
        <li>HTML</li>
        <li>CSS</li>
        <li>DOM Manipulation (Document Object Model)</li>
        <li>Event Listeners</li>
        <li>Programming Logic</li>
        <li>Math Operations</li>
        <li>Objects in JavaScript</li>
        <li>Functions in JavaScript</li>
        <li>and more...</li>
    </ul>
        </ul>
    </div>
        <br>
        <a href="https://angnz.github.io/SimpleOS/lvl1/2023/10/18/simple-background-color.html">➡️ Code</a><br>
        <a href="https://angnz.github.io/SimpleOS/lvl1/">➡️ lvl1</a>
</div>

<div class="fenster_lvl2">

    <p class="fenster-letters"><h2>Lvl 2: Simple Product showcase</h2>
    <hr><br> A simple Product showcase in html, JS, and CSS.<br>It contains:</p>

    <div class="console">
        <ul>
        <li>Shop Cart</li>
        <li>Alphabetical Order of Products</li>
        <li>Add to Cart Button</li>
        <li>Generate Product Segments</li>
        <li>Sum and Subtract Prices</li>
        <li>Personal Data Form</li>
        <li>Send Quotation via Email</li>
        </ul>
    </div>
        <br>
        <a href="http://petitaideas.com/test/">➡️ See it in acction</a><br>
        <a href="https://angnz.github.io/SimpleOS/ssc/">➡️ Code</a>
</div>

# Research and Data

<div class="fenster">

    <p class="fenster-letters"><h2>Research & Data Science</h2>
    <hr><br> Data science fundamentals for Socioeconomical studies</p>

    <div class="console">
        <ul>
        <li>16.10.23 Introduction</li>
        </ul>
    </div>
        <br>
        <a href="https://angnz.github.io/SimpleOS/ds-economics/">Go to more Data</a><br>
</div>

# Programming

<div class="fenster">

    <p class="fenster-letters"><h2>Programming & Analytics</h2>
    <hr><br> Data science fundamentals for Economics and Social Sience</p>

    <div class="console">
        <ul>
        <li>JavaScript</li>
        <li>SPSS</li>
        <li>Phython</li>
        <li>VBA</li>
        <li>R</li>
        </ul>
    </div>
        <br>
        <a href="https://angnz.github.io/SimpleOS/ds-economics/">➡️ Go to Data</a><br>
</div>




[Chek how did I create this page](Jekyll/)

{% for post in site.posts limit:0 %}
   <article>
      {% include article.html %}
    </article>
{% endfor %}

