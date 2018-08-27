## Organising your page

So far you've used **headings** and **paragraphs** to make your **content** look tidy and easy to read. Let's make it even more organised by grouping things together.

--- collapse ---
---
title: What is content?
---

**Content** is all the stuff on your web page, such astext and pictures.

--- /collapse ---

+ Go to the `birds.html` file (or one of your own pages if you're not using the example project) and, near the top, just **below** the opening `<main>` tag, type the following on a new line: 

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
      <h1>Birds of conservation concern in Ireland</h1>
      <p>
       There are a number of birds in Ireland whose numbers are in decline.
       Some of those with a high priority for conservation are:
      </p>  
      
      <h2>Barn Owl</h2>
      <p>The barn owl is the most common owl and is found in most parts of the world. 
      It has seen a huge decline in Ireland and Europe in recent years.</p>
      <img src="barn-owl-landing.jpg" alt="Barn owl landing on a branch" height="200px" />
      <h2>Curlew</h2>
      <p>The curlew is recognisable by its long curved bill.
      </p>
      <img src="curlew.jpg" width="200px" />
      <p>Curlews use their long bills to search for worms in mud or very soft ground.
      </p>
      <img src="curlew2.jpg" width="200px" />
    </article>
  </main>
```

+ Now look at the content in your `article` and try to break it up into sections. Put this new pair of tags around each bit: `<section> </section>`. Here's an example of what it might look like:

```html
  <article>
    <h1>My favourite places to see in Ireland</h1>
    <section>
      <h2>Barn Owl</h2>
      <p>The barn owl is the most common owl and is found in most parts of the world. 
      It has seen a huge decline in Ireland and Europe in recent years.</p>
      <img src="barn-owl-landing.jpg" alt="Barn owl landing on a branch" height="200px" />
    </section>
    <section>
      <h2>Curlew</h2>
      <p>The curlew is recognisable by its long curved bill.
      </p>
      <img src="curlew.jpg" width="200px" />
      <p>Curlews use their long bills to search for worms in mud or very soft ground.
      </p>
      <img src="curlew2.jpg" width="200px" />
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

Look at the Conservation page of the example project. You'll see that I've added an `article` with a bunch of `section` tags into the file `conservation.html`:

```html
  <main>
	    <article>
	    
  	    <h1>Conservation efforts</h1>
        <p>
         Various kinds of work are carried out in Ireland in order to protect bird species.
        </p>  
        
        <section>
          <h2>Research and monitoring</h2>
          <p>
            An essential part of bird conservation is monitoring and recording 
            information about the species such as their numbers, breeding habits, etc. 
        
          </p>
          <p>
            Scientific research may be carried out to determine whether a species is 
            in decline and how to address the problem.
          </p>
        </section>
        
        <section>
          <h2>Habitat protection</h2>
          <p>
            The destruction of habitat is a serious threat to many birds and 
            therefore protecting habitats is crucial to protecting the species.
          </p>
          
          <p>One example of this is the preservation of wetlands in Ireland.</p>
        </section>
        
        <section>
          <h2>Control invasive plants and animals</h2>
          <p>
            Mink and rats are a predator that threaten many bird species, 
            for example by eating their eggs.
          </p>
          <p>
            Rhododendron is an example of an invasive plant which can very quickly
            take over large areas of countryside, disrupting the biodiversity.
          </p>
        </section>
	    </article>   
  </main>
```

--- /hint ---

--- /hints ---

On the next card, you'll design a different theme for each page that's organised into articles and sections!

--- /challenge ---
