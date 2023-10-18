---
layout: post
title:  "Simple Backgrund color"
date:   2023-10-18 21:42:47 +0200
categories: lvl1
---

# Topics for creating the Background color changer

- JavaScript
- HTML
- CSS
- DOM Manipulation (Document Object Model)
- Event Listeners
- Programming Logic
- Math Operations
- Objects in JavaScript
- Functions in JavaScript
- Data Validation
- State Management
- Rounding Numbers
- Debugging and Testing

# HTML

This HTML code creates a basic webpage with the following elements:

- A document declaration specifying that this is an HTML5 document.
- A head section with character encoding and viewport meta tags.
- A title for the webpage.
- The body of the webpage contains an <h1> heading that says "Backgrund color" and a <div> element with three buttons labeled "Red," "Yellow," and "Black." These buttons have unique IDs ("btn_red," "btn_yellow," and "btn_black").

{% highlight html  %}

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    
    <title>Document</title>
</head>

<body>

    <h1>Backgrund color</h1>
    <div class="wrapper">
        <button id="btn_red">Red</button>
        <button id="btn_yellow">Yelow</button>
        <button id="btn_black" >Black</button>
    </div>


</body>
</html>


{% endhighlight %}

# CSS

{% highlight css  %}

<style>
        button {
            border-radius: 5px;
            background: grey;
            color: black;
            border: solid 1px var(--white);
            text-decoration: none;
            cursor: pointer;
            font-size: 1.2em;
            padding: 18px 10px;
            width: 180px;
            margin: 10px;
            outline: none;
        }

        button:hover {
            transition: all 0.5s ease-in-out;
            background: var(--white);
            border: solid 1px var(--white);
            color: var(--base-color);
        }

        #red {
            background-color: red;
        }

        #yellow{
            background-color: yellow;
        }

        body {
            background-color: whitesmoke;
            transition: background-color 0.5s; /* Add transition for smoother color change */
        }
    </style>

{% endhighlight %}

# JS

This JS code creates a basic webpage with the following elements:

- It selects three HTML elements with the IDs "btn_red," "btn_yellow," and "btn_black" and assigns them to variables.
- It gets a reference to the <body> element and assigns it to the body variable.
- It adds event listeners to each of the three buttons.
- When "btn_red" is clicked, it changes the background color of the body to red and styles the button with a red background and white text.
- When "btn_yellow" is clicked, it changes the background color of the body to yellow and styles the button with a yellow background and white text.
- When "btn_black" is clicked, it changes the background color of the body to black and styles the button with a black background and white text.
- In summary, this code allows you to change the background color of the webpage by clicking on one of the three buttons, each corresponding to a different color (red, yellow, or black).

{% highlight javascript  %}

    <script>
        let btn_red = document.getElementById("btn_red");
        let btn_yellow = document.getElementById("btn_yellow")
        let btn_black = document.getElementById("btn_black")

        var body = document.body;

        btn_red.onclick = function () {
            body.style.backgroundColor = "red"; // Change the background color of the body to red
            btn_red.style.backgroundColor = "red"
            btn_red.style.color = "white"
        }

        btn_yellow.onclick = function() {
            body.style.backgroundColor = "yellow"
            btn_yellow.style.backgroundColor = "yellow"
            btn_yellow.style.color = "white"

        }

        btn_black.onclick = function () {
            body.style.backgroundColor = "black"
            btn_black.style.backgroundColor = "black"
            btn_black.style.color = "white"
        }

    </script>

{% endhighlight %}