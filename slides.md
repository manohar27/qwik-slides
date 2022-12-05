---
theme: default
layout: intro
highlighter: shiki
lineNumbers: false
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
drawings:
  persist: false
css: unocss
title: Qwik fix to the cost of javascript
---

# Qwik fix to the cost of javascript

Introduction to the new web framework

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Let's Begin <carbon:arrow-right class="inline"/>
  </span>
</div>

<!--
This is not an ad

There are some questions for you during our session, use teams chat

Repo used here will be shared if you want to try it out
-->

---

# Intro

<img style="margin-left: 16px; border-radius: 50%" src="https://manohar27.github.io/static/c1964f6e2e0ba238580438fce033b3d6/9067c/profile-pic.jpg" width="100" alt="profile-pic" />
<br>

- Manohar Srinivasa
- **SDE-2** with Digital Content Experience Platform building <img style="display: inline" src="https://digitalcontent.api.tesco.com/v2/media/test/94f69ef8-8555-4fe6-b5f0-603d19558d03/tesco-logo-fill.png?h=25" alt="spectra-ui" height="100"/>
- **6.5** years in Tesco

<br>
<br>

<a href="mailto:manohar.srinivasa@tesco.com">✉️ manohar.srinivasa@tesco.com</a>

[🌐 manohar27.github.io](https://manohar27.github.io)

<!--
Remember to start recording
-->

---
layout: section
---

# Evolution of web development

<!--
Quick recap of how things were
-->

---
layout: image-right
image: /assets/mohammad-rahmani-oXlXu2qukGE-unsplash.jpg
---

# Remember this?

```php {|6}
<html>
 <head>
  <title>PHP Test</title>
 </head>
 <body>
 <?php echo '<p>Hello World</p>'; ?>
 </body>
</html>
```

<v-click>

<br />

* Multi page applications
* Any interaction was a page reload
* Zero javascript

</v-click>

<!--
Imagine like a tweet causing a page reload
-->

---
layout: default
---

# And these?

<v-click>
<img class="inline m-4" src="/assets/ruby-on-rails.webp" width="100" />
</v-click>
<v-click>

<img class="inline m-4" src="/assets/xampp.png" width="100" />
</v-click>

<v-click>

<img class="inline m-4" src="/assets/django.png" width="100" />
</v-click>


<v-click>

<img class="inline m-4" src="/assets/vaadin.png" width="100" />
</v-click>

<v-click>

#### and everything else
</v-click>

<v-click>

<img class="inline m-4" src="/assets/all-the-frameworks.jpg" />
</v-click>

<!--
And as web got more and more interactive
-->

---
layout: two-cols
---

# Land of javascript

* jquery
* polymer
* ember
* backbone
* angular
* reactjs - nextjs, gatsby
* vuejs
* svelte
* etc

::right::

<v-click>
<img src="/assets/meme-1.jpeg" >
</v-click>

<!--
etc includes qwik as well
-->

---

# Quiz

<h3>What is the popular python based web framework <logos-python /> ? </h3>

a) polymer

b) vaadin

c) django

d) qwik

<br/>

### Answer
<v-click>
<h1 class="c-green">django</h1>
</v-click>

<!--
Let's use the team chat to leave your answers
-->

---
layout: two-cols
---

# Cost of javascript


* Complexity ⏫ = Javascript ⏫
* Download time
* Parsing
* Hydration


<v-click>

## This leads to

* Impact on revenue
* Impact to SEO

</v-click>

<v-click>

## You then try to solve it

* Devs figuring out how to split bundles
* Inlining critical css,js - lazy loading everything else

</v-click>

::right::

<v-click>
<h2>An example <logos-reddit /> </h2>

<br />
<img src="https://v8.dev/_img/cost-of-javascript-2019/reddit-js-processing.svg">

<quote class="c-blue">Source: v8.dev (2019)</quote>
</v-click>

<!--
Javascript is proportional to the complexity

Revenue - customers will leave if your site is slow

Page speed impacts SEO ranking
-->

---
layout: two-cols
---

# Another example: tesco.com

## Quiz 

<br />

### Any guesses on what tesco.com's webvitals performance score is? 

Post your guesses in the teams chat




::right::


<v-click>

## Answer
</v-click>

<v-click>

* Mobile

<img src="/assets/mobile.png" width="250"  >


<br />

* Desktop

<img src="/assets/desktop.png" width="250" >
</v-click>

<!--
Yeah there's room for improvement here

JS is the enemy

The Time to Interactive is about 12s on a mobile device
-->

---
layout: section
---

# Qwik

---
layout: two-cols
---
<h1><span class="c-blue">qwik</span> is a</h1>

<br/>

* ## resumable
* ## progressive 

UI framework built by builder.io

<br />
<h3>
<a href="https://qwik.builder.io/">https://qwik.builder.io/</a>
</h3>

::right::

<img src="/assets/qwik-start.png"  />

---
layout: center
---

# So what's different ?

* ## Delaying JS execution as much as possible
* ## Resumability

<!--
Also called progressive
-->

---

# Delay JS execution

<br />

<img style="width: 100%" src="/assets/qwik-overview.png" />

<!--
qwik loader, bare minimum js for qwik to start
-->

---

# Resumability
<img src="/assets/hydration-resumable.webp" />

<!--
two versions - html & js component tree

component tree event mapping/binding
-->

---
layout: section
---

<h1> Hands on </h1>

<v-click>
<div style="display: flex; justify-content: center">
<img width="400" src="/assets/demo-god-meme.jpeg" />
</div>
</v-click>

---
layout: iframe-right
url: https://todo-app-qwik.vercel.app/
---

# Timed todo app

<br />

#### Let's implement delete todo functionality


<br />
<br />

<logos-github-icon /> <a class="text-[0.8em]" href="https://github.com/manohar27/todo-app-qwik">https://github.com/manohar27/todo-app-qwik</a>

<br />
<br />


<p class="text-[0.8em]">

P.S: There's a very easy to find easter egg in the application, let's see who finds it first. Post a screenshot in the teams chat

Scan the below QR code to open the app on your phone

<img width="100" src="/assets/todo-app-vercel.png" />

</p>

<!--
Show the timer feature

Find the easter egg

Send the url on chat

Show that No JS is downloaded on live

Show that progressively JS is downloaded


Watch out for time here

Open dev version


Show qwik loader

Show QRL - qwik optimizer

Show progressive nature

Show code that is downloaded

Show resumability with HTML copy paste in new tab

Start from todo-list/index

implement delete functionality


If there is time, go through simple counter example
-->

---
layout: section
---

# Questions?


---
layout: intro
---

# Thank you

