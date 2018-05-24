## Automatically adjust the size

Up until now you've been using **pixels** to set the size of things, e.g. `10px`. On this card you will learn about other measurements you can use.

+ Go to `index.html` and find the `img` element with the picture of the barn owl, or find another `img` tag on your website.

+ Delete the `width` attribute if it's there, and give the element an `id` if it doesn't already have one.

```html
  <img src="barn-owl.jpg" id="owly" alt="A barn owl" />
``` 

+ In your CSS file, define the `width` property for your picture as shown below (you might need to create the CSS block with the `id` selector if you haven't already done so on a previous card).

```css
  #owly {
    width: 50%;
    border-radius: 100%;
  }
```

Note: 50% (50 percent) is **half**. 

+ Try resizing your browser window and watch what happens to the picture.

You should see that the picture gets bigger and smaller when you make the window bigger and smaller. That is because it is taking up 50% of the width of the **main** element (which is roughly the width of the page).

--- collapse ---
---
title: How does it work?
---

When you set the size of something in pixels, you are setting an exact size and it doesn't change. This is called an **absolute** measurement. 

Another way to set the size of things is using **relative** measurements, so that size depends on how big elements are compared to each other. Then, whenever one thing changes size, everything else will automatically change size as well to keep the same **proportions**. 

When you're using **relative** measurements, it's important to know what the **parent** of your element is. The parent is the thing that your element is inside of, and that's what the measurement will be in relation to. For example, the parent of the image above is the `article` element, because the `img` element is in between the `<article></article>` tags.

If you set the `width` of an element to `100%`, that will make it be the same width as the parent container it's in.

--- /collapse ---

+ Experiment with different numbers in front of the `%`.
