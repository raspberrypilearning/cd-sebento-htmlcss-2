## Organising your page

So far you've used **headings** and **paragraphs** to make your **content** look tidy and easy to read. Let's make it even more organised by grouping things together.

--- collapse ---
---
title: What is content?
---

**Content** is all the stuff on your web page, such astext and pictures.

--- /collapse ---

+ Go to the `attractions.html` file (or one of your own pages if you're not using the example project) and, near the top, just **below** the opening `<main>` tag, type the following on a new line: 

```html
  <main>
    <article>
```

+ If your editor automatically added in a closing `</article>` tag for you, delete it.

+ At the bottom of the file, just **above** the closing `</main>` tag, add a new line and close the `article` element:

```html
    </article>
  </main>
```

Your `main` element should look something like this now (you might have different content in between the `article` tags of course):

```html
  <main>
    <article>
      <h1>My favourite places to see in Ireland</h1>
        <h2>The Cliffs of Moher</h2>
        <p>
        The Cliffs of Moher are found in County Clare, where I am from. Look how cool they are!</p>
        <img src="cliffs.JPG" alt="The Cliffs of Moher" height="200px" />
        <h2>Achill Island</h2>
        <p>This is a large island off the coast of County Mayo. It has a wild and
        beautiful landscape of mountains, bogs and cliffs.
        </p>
        <img src="achill.JPG" width="200px" />
    </article>
  </main>
```

+ Now look at the content in your `article` and try to break it up into sections. Put this new pair of tags around each bit: `<section> </section>`. Here's an example of what it might look like:

```html
  <article>
    <h1>My favourite places to see in Ireland</h1>
    <section>
      <h2>The Cliffs of Moher</h2>
      <p>
      The Cliffs of Moher are found in County Clare, where I am from. Look how cool they are!</p>
      <img src="cliffs.JPG" alt="The Cliffs of Moher" height="200px" />
    </section>
    <section>
      <h2>Achill Island</h2>
      <p>This is a large island off the coast of County Mayo. It has a wild and
      beautiful landscape of mountains, bogs and cliffs.
      </p>
      <img src="achill.JPG" width="200px" />
    </section>
  </article>
```

--- collapse ---
---
title: What are the new tags all about?
---

Think of these new elements as **containers**. They are used to group things together. It's a bit like organising things in boxes and shelves in your home! 

This makes your website friendly for screen readers, gives you more control over the layout, and, as you'll see, it allows you to really get creative with the styling.

Anything can go in between the tags. Usually it will be more than one element, but it doesn't have to be. It can be HTML elements of any kind. What you are doing is telling the browser that everything in between these tags belongs together. 

### Article

The `article` element is a container for a whole piece of content, in this case a set of information about attractions in Ireland. If you have different bits of content that aren't related, you should put each one into its own `article` element instead of putting one set of the tags around the whole lot.

### Section

The `section` element lets you divide up related content into smaller chunks and put each chunk into its own container.

### Others exist too!

These aren't the only container elements in HTML. If you've ever created a menu and then put it in between `<nav> </nav>` tags, that's another example of a type of container. So are `<main> </main>` and `<header> </header>` — can you think of any more?

--- /collapse ---

--- challenge ---

Your web page might not look different yet, but once the content has been organised into container tags, you'll be able to do some cool things to it with CSS. Remember, HTML controls how your website is organised, and CSS controls how it looks. 

## Challenge: organise your website

+ Have a go at organising all of the content on your website using the `article` and `section` containers in this way. 

--- hints ---

--- hint ---

Look at the Food page of the example project. You'll see that I've added an `article` with a bunch of `section` tags into the file `food.html`:

```html
  <main>
    <article>
      <h1>Food in Ireland</h1>
      <p>
        These are some of my favourite Irish foods!
      </p>  
      <section>
        <h2>Traditional Irish Breakfast</h2>
        <p>
          A "Full Irish" breakfast consists of sausages, rashers (bacon),
          eggs, black pudding, white pudding and toast.
        </p>
        <p>
          Often there will be a grilled tomato as well as mushrooms,
          and baked beans.
        </p>
        <p>
          And of course, no breakfast is complete without a lovely pot 
          of tea!
        </p>
      </section>
        
      <section>
        <h2>Bangers and Mash</h2>
        <p>
          This classic of sausages, mashed potato and gravy is not
          unique to Ireland, but what makes it special is the Irish
          sausages. Most countries have their own way of making sausages,
          and they are one thing I miss from home if I'm away travelling!
        </p>
      </section>
        
      <section>
        <h2>Bacon and Cabbage</h2>
        <p>
          I couldn't possibly make a list of Irish food without including
          this very traditional dish!
        </p>
        <p>
          It might not sound very interesting, but this hearty meal of
          boiled ham, potatoes and green cabbage is tasty and filling.
          I love to smother the potatoes in butter, and I also like a
          little mustard with the bacon.
        </p>
        <p>
          My mum always made it extra special by cooking the cabbage in
          the water that the ham was boiled in.
        </p>
        <p>
          If there are any leftovers you can make another one of my
          favourites: <strong>fried cabbage</strong>!
        </p>
      </section>
    </article>     
  </main>
```

--- /hint ---

--- /hints ---

On the next card, you'll design a different theme for each page that's organised into articles and sections!

--- /challenge ---
