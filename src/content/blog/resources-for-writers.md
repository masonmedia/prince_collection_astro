---
draft: true
title: Resources for writers
author: Andrew Mason
description: A list of FAQ, trouble shooting tips, and image grid code snippets.
SEOdescription: Ipsum Lorem velit eu deserunt magna cupidatat eiusmod esse elit in.
pubDate: 2024-03-01T18:44:56.087Z
imageUrl: /images/uploads/belmond-bellini-review-2.png
imageAlt: Add image alt text = this same text will be applied to the carousel if used
category: blog
tags:
  - four-seasons
  - seattle
  - hotels
carousel:
  - url: /images/uploads/belmond-bellini-review-2.png
  - url: /images/uploads/belmond-bellini-review-10.jpeg
  - url: /images/uploads/belmond-bellini-review-9.jpeg
gallery: []
contents:
  - html-3x-grid
  - ridiculus-mus-mauris-vitae
  - html-image-using-figure-and-caption
  - faucibus-nisl-tincidunt
  - another-h2
---

# Resources for writers


- - -


# Main post title


Make post title an H1 and all subsequent headings H2. If using an unordered (bullet) list subtitles can be H4.


### Adding images and image grids


Copying and pasting the code snippets below allows writers to add image galleries to posts. 


> **It's important to copy and paste the code exactly as written, and take care to be sure there are no extra characters, periods, commas, back ticks, etc. They will cause errors on the front end when published.**


*\*Occasionally the editor will add characters to raw HTML especially backslashes but watch for periods, commas, etc.*


### Steps


* Copy desired gallery code from below.
* Select "Markdown" from the top right toggle switch.
* Paste code where you want it in the article
* add image file paths (see below)
* ensure there are no typos
* return to Rich Text editor (toggle Rich Text in top right select)


### Naming images


* First, name all your article images **before** uploading them to the CMS. 
* This keeps the image library clean and organized, and prevents rogue images with names like IMG_32459875 that are impossible to keep track of.
* use a convention like the following: **article-name-1.jpeg** i.e. waldorf-astoria-cabo-san-lucas-1.jpeg, waldorf-astoria-cabo-san-lucas-2.jpeg
* this allows you to search images in the media folder for ease of selection throughout the writing process
* Add/upload ONLY images you actually use. This keeps the site payload as small and efficient as possible.


### Uploading images


* Upload all images (you can do this either using the featured image field, or you can add an image widget to a post, and add all images from there once you access the media library)
* Do not leave an empty image widget in your post => it will break the page/site


### Adding images to your grid gallery


* add an image widget (from the top menu/toolbar click the + and a dropdown will appear, select "Image") above or below your gallery code, just to use as a way to select images from the library
* open the media library
* find your image and click it to highlight
* in the upper left button toolbar, select **"Copy Name"**: this will give you the name of the file i.e. waldorf-astoria-cabo-san-lucas-1.jpeg
* in cases it will only allow you to select **"Copy Path"**: this will give you the full file path: public/images/uploads/waldorf-astoria-cabo-san-lucas-1.jpeg. In this case you have to **delete the "public"** part from the path.
* final image url should look like: 
  **/images/uploads/waldorf-astoria-cabo-san-lucas-1.jpeg**


**<img src="/images/uploads/waldorf-astoria-cabo-san-lucas-1.jpeg" />**


<figure>
   <img class="grid-image" src="/images/uploads/waldorf-astoria-cabo-san-lucas-1.jpeg" alt="" />
</figure>


### 2-column grid


This gallery creates a 2-column side-by-side grid. You can also add 4 images like below to get a 4-grid gallery. 


<div class="grid-2">
  <figure>
        <img class="grid-image" src="/images/uploads/brando-2.jpeg" alt="" />
    </figure>
    <figure>
        <img class="grid-image" src="/images/uploads/brando-2.jpeg" alt="" />
    </figure>
</div>


<div class="grid-2">
  <figure>
     <img class="grid-image" src="/images/uploads/brando-2.jpeg" alt="" />
  </figure>
  <figure>
     <img class="grid-image" src="/images/uploads/brando-2.jpeg" alt="" />
  </figure>
  <figure>
     <img class="grid-image" src="/images/uploads/brando-2.jpeg" alt="" />
  </figure>
  <figure>
     <img class="grid-image" src="/images/uploads/brando-2.jpeg" alt="" />
  </figure>
</div>


### 3-column grid


This gallery creates a 3-column side-by-side grid. The drawback to this variation is the images are a little small. Best to use for instances where images have lower content/meaning, plane window, runway, arrival, etc.


<div class="grid-3">
  <figure>
     <img class="grid-image" src="/images/uploads/brando-2.jpeg" alt="" />
    </figure>
    <figure>
        <img class="grid-image" src="/images/uploads/brando-2.jpeg" alt="" />
    </figure>
    <figure>
        <img class="grid-image" src="/images/uploads/brando-2.jpeg" alt="" />
    </figure>
</div>


### One big, two small


This gallery creates a big feature image with two smaller images side-by-side underneath it.


<div class="one-big-two-small">
  <figure>
        <img class="grid-image" src="/images/uploads/brando-2.jpeg" alt="" />
    </figure>
    <figure>
        <img class="grid-image" src="/images/uploads/brando-2.jpeg" alt="" />
    </figure>
    <figure>
        <img class="grid-image" src="/images/uploads/brando-2.jpeg" alt="" />
    </figure>
</div>


## Using figure and figcaption


If desired you can copy/paste the `<figcaption>`element which adds a text description of the image just below it. **It isn't necessary and if used needs to be added to every other image in the grid so it doesn't a) look imbalanced, and b) misalign spacing.**


<figure>
    <img src="/images/uploads/brando-2.jpeg"
         alt="Albuquerque, New Mexico">
    <figcaption>A single track trail outside of Albuquerque, New Mexico.</figcaption>
</figure>


## Making a table of contents


Every title in your post gets converted into an `id` that can be used as an anchor for in-article navigation. The subtitle ***Making a table of contents*** becomes `<h2 id="making-a-table-of-contents">Making a table of Contents</h2>` automatically. This then gets added to a menu at the top of the page that links that each specific title in the article.


To activate the table of contents at the start of the post, copy and paste each article heading/subtitle into the **"Table of Contents"** field just above the article body widget. Add a single comma (which automatically creates a space) to add the next title (don't use the spacebar). You can link as many titles as you want, just be aware that this will directly impact the size of the visible table of contents in the post.


## Lists


* Lists are given global styling in the theme code
* Bullet lists are given unique icons for bullets 
* They are laid out in a 2x grid for more attractive styling and to take up less space


## Text layout


For ease of reading and UX expectation, avoid short sentences broken into unique lines as a general post writing style. It makes it difficult to know where a main concept/section starts and ends, and gives the page a disjointed look more akin to a list than an article.
