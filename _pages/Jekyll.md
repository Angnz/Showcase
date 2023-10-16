---
layout: page
permalink: /Jekyll/
title: ":Jekyll webPage"
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

## How I create this Page in Jekyll
There are 2 ways to add code to HTML without JS:
- `<pre>`
- `<code>`

## In Kekyll
```
your code
```
The example below will use code with some CSS for formatting, otherwise it looks like shit.


## Uploading to GitHub from VSCode using Git commands MTF's

- To check if the server is connected, use: 
```
$ git config --global --list
```
- To update:
```
$ git push
```
- To initialize a repository:
```
$ git init
```
- To add files to your repository: (Here, "Home.html" is an example)
```
$ git add Home.html
```
- To add a commit message:
```
$ git commit -m "I uploaded the first HTML page as Home"
```
<div class="messagebox"> Just learned how to upload stuff from VSCode to GitHub using Git commands.</div>

## How to rename files using Git from VSCode

- Rename a file:
```
git mv old-file.html new-file.html
```
- Commit it:
```
git commit -m "Renamed old-file.html to new-file.html"
```
- Update it:
```
git push
```

<div class="messagebox">
With these commands, you can easily rename files in your repo on GitHub.
</div>
