---
layout: layouts/swordFish.njk
title: swordFish
date: 2017-01-01T00:00:00.000Z
permalink: /swordFish/index.html
footerMsg1: hello from var footerMsg1 in swordFish.md
eleventyNavigation:
  key: swordFish
  order: 5
---
hello from swordFish file: eleventy-netlify-boilerplate/pages/swordfish.md

> ya gotta stuff pics in folder: static/img/  
>eleventy.js has some passthrough logic to upload those images to netlify. 

>here is imbedded html in the markdown file:
 
<img src="../static/img/img_girl.jpg" alt="Girl in a jacket" width="250" height="300">

>I tried inserting the image with markdown instead of imbedded html,
but the image cant be resized.  this duznt work right:
 ``    ![GirlieJacket](/static/img/img_girl.jpg){width=50% height=50% } ``
this works, but who cares?  ``    ![GirlieJacket](/static/img/img_girl.jpg) ``
> what a hassle.  


Leave the fancy formatting (css) to the web programmer.

> elventy has a cute possum balloon thing.  Here's my take on it:
<img src="../static/img/possumBalloonRoadside.jpg" alt="PossumBalloon" width="250" height="300">

> wow, markdown is so much fun.  
Notice the reams of stack overflow questions on it.  
I am not feeling the love. 

> In the top of markdown files, chris coyier uses front matter: 
https://jekyllrb.com/docs/front-matter/ 
See the top of this file, between the three dash lines.  
I notice  github has some awareness of the front matter stuff in a .md file.

>Below is text with a css class of selzClass1

>my text line in markdown with class {.selzClass1}
>I added a markdown plugin:
https://www.npmjs.com/package/markdown-it-attrs
https://www.11ty.io/docs/languages/markdown/#add-your-own-plugins
The intent was to identify the css class when writing in markdown.
But this pollutes markdown.  A purist wants very little in the markdown. Mostly just text.
> I expanded 11ty to get css class to work.
package.json I added markdown-it-attrs to refrence the module
 eleventy.js I added markdown-it-attrs to require the module
 
``` bulma change color {.has-text-primary} ```
bulma change color {.has-text-primary}

> the end of ```swordfish.md ```
