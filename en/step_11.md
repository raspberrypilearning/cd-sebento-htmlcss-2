## Add hover effects

You can make your website more **interactive** by making cool stuff happen when you hover over things with the mouse cursor! 

+ Find your CSS rules for the `img` elements, or create some if you don't have any. Add in a border, and then add a new block of rules right below:

```css
  img {
    border: 2px solid White;
  }
  img:hover {
    border: 2px dashed Navy;
  }
```

You've just used a special type of CSS block called a **pseudo-class**.

--- collapse ---
---
title: How does it work?
---

A **pseudo-class** is a bit different from a **class** that you create yourself. You can recognise it by the `:`.

Pseudo-classes come built in to HTML elements: you can add `:hover` style rules to any element, class, or `id` selector in your style sheet without needing to add anything extra in your HTML code.

--- /collapse ---

+ What do you think will happen? Check what pages on your website have pictures on them (add a picture if there aren't any!), then move your cursor over a picture to find out!

+ Let's use this new `:hover` pseudo-class together with a CSS class to make links glow when you hover over them! Add a link to your web page and include an attribute to specify the class name. Remember, links are defined using the `<a>` tag, like so:

```html
    <p>
      <a class="niceLinks" href="https://en.wikipedia.org/wiki/Bird_conservation">Click here</a> 
        to read about bird conservation on Wikipedia.
    </p>
```

+ Add the following code to your style sheet, then run your code to see your lovely links in action.

```css
  .niceLinks {
    text-decoration: none;
    color: #FFFAF0;
  }
  .niceLinks:hover {
    color: #00FF7F;
  }
```

+ Why not add the attribute `class="niceLinks"` to all of the links in your menu bar as well?

You can combine all of these tricks with animations too! 

+ Find the CSS block for the picture of the barn owl again (or whatever picture you were working on earlier). Add the following code to your style sheet file:

```css
  #owly {
    border-radius: 100%;
    width: 100px;
  }
  #owly:hover {
    animation-name: rollOver;
    animation-duration: 1s;
    animation-iteration-count: 1;
  }
  @keyframes rollOver {
    0% {
      transform: rotate(0deg);
    }
    100% {
      transform: rotate(-360deg);
    }
  }
```

+ Can you guess what will happen?

+ Move the cursor over the picture to find out!

--- challenge ---

## Challenge: make glowing rainbow links

+ Can you use the `rainbowGlow` animation from the previous card to make the links in your menu keep changing colours when the cursor is hovering over them?

--- hints ---

--- hint ---

Below is the code for the `rainbowGlow` animation. It has five stages defined, and it sets a different text colour at each stage. You can add more or change them however you want!

```css
    @keyframes rainbowGlow {
        0% {
            color: #00BFFF;
        }
        25% {
            color: #00FF7F;
        }
        50% {
            color: #eeeeaf;
        }
        75% {
            color: #eeafee;
        }
        100% {
            color: #00BFFF;
        }
    }
```
   
--- /hint ---

--- hint ---

To animate something, you add the three `animation` properties to its style rules as you've done above. Always make sure the `animation-name` matches the name of the animation you wish to use.

--- /hint ---

--- hint ---

You can add `hover` effects directly to the `nav` menu like this:

```css
  nav ul li a:hover {
    animation-name: rainbowGlow;
    animation-duration: 1.5s;
    animation-iteration-count: infinite;
  }
```

Or, if you want to make other links on your website flash rainbow colours too, you can add the animation to the `.niceLinks` class instead, like this:

```css
  .niceLinks:hover {
    color: #00BFFF;
    animation-name: rainbowGlow;
    animation-duration: 1.5s;
    animation-iteration-count: infinite;
  }
```

--- /hint ---

--- /hints ---

--- /challenge ---

