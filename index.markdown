---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

<style>
body {
    font-family: Arial, sans-serif;
    background-color: #1F4172;
    margin: 2em;
    padding: 1em;
}

.site-header{ /*site-header is the Webpage Banner and  text*/
    Color: #132043;
    font-family: Arial, sans-serif;
    background-color: #363062;
    
}

.divheader {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 20px;
}

.fenster {

    background-color: #F5F5DC; /* Color azul crema */
    border-radius: 5px; /* Bordes redondeados */
    box-shadow: 5px 5px 5px #888;
    max-width: 960px;
    margin: 0 auto;
    padding: 20px;
    margin-top: 1em;
}

fenster-letters{

    color:#333;
}
button {
    background-color: #0074d9;
    color: #fff;
    padding: 10px 20px;
    border: none;
    cursor: pointer;
}

code {
    font-family: 'Courier New', Courier, monospace;
    color: #333;
    background-color: #f4f4f4;
    border: 1px solid #ddd;
    border-radius: 5px;
    padding: 10px;
    font-size: 16px;
    line-height: 1.5;
    overflow-x: auto;
}

li {
    line-height: 3em;
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


# Angelus
## Welcome to SimpleOS Hier are some projects I am currently working on:
- Peitaideas


<div class="fenster">
<p class="fenster-letters"><h2>Peitaideas Online Shop.</h2><br> A simple shop in html, JS, and CSS</p>
<p>
It contains:
<ul>
    <li>Shop Chart</li>
    <li>Alhabetical order of products</li>
    <li>Add to Chart button</li>
    <li>Generate Products Segments</li>
    <li>Summ and Substracts price</li>
    <li>Personal Data form</li>
</ul>

</p>
<a href="http://petitaideas.com/test/">See it in acction</a>
Code: <a href="https://angnz.github.io/SimpleOS/pi/">Click hier</a>
Code: <a href="https://angnz.github.io/SimpleOS/contact/">Contact</a>
</div>


[Link to the PI Page](pi/)

## There are 2 ways to add code to HTML without JS:

- `<pre>`
- `<code>`
## In Kekyll

```

your code

```

<div class="messagebox">
  The example below will use code with some CSS for formatting, otherwise it looks like shit.
</div>

## Uploading to GitHub from VSCode using Git commands MTF's

- To check if the server is connected, use: `$ git config --global --list`
- To update: `$ git push`
- To initialize a repository: `$ git init`
- To add files to your repository: `$ git add Home.html` (Here, "Home.html" is an example)
- To add a commit message: `$ git commit -m "I uploaded the first HTML page as Home"`

<div class="messagebox"> Just learned how to upload stuff from VSCode to GitHub using Git commands.</div>

## How to rename files using Git from VSCode

- Rename a file: `git mv old-file.html new-file.html`
- Commit it: `git commit -m "Renamed old-file.html to new-file.html"`
- Update it: `git push`


<div class="messagebox">
With these commands, you can easily rename files in your repo on GitHub.
</div>

Here's my stuff.
<button id="btndemierda">A la mierda</button>


<script>
document.getElementById("btndemierda").addEventListener("click", function() {
    alert("Me has clickeao, Tio"); 
});
</script>
