# Netflix Clone

Clone of the Netflix website as a light HTML CSS and JS excercise -

[![Practice](https://img.shields.io/badge/Practice-HTML/CSS/JS-orange.svg)]

_<p align="center">"Eating website for fun... nyom nyom nyom"</p>_

<div align="center" style="text-align:center; margin:auto;">
<img align="center" src="https://i.imgur.com/EgCvXyK.png" width="150"/>
</div>

## What it is

A basic warmup exercise. Simple, practice oriented, clone of the Netflix Homepage. Built with:

- HTML
- CSS
- Vanilla JS - ES6

## What it does

- Look pretty, that's about it :-)

## Learning Points

- CSS Grid
- Styling Tables
- Tabs with Javascript
- Positioning

## Some cool stuff

Usually, people tend to run to CSS Frameworks to develop and style tabs and switching tabs. But here's a pretty simple, basic way of creating switchable tab content using Vanilla JS:

```javascript
const tabItems = document.querySelectorAll(".tab-item");
const tabContentItems = document.querySelectorAll(".tab-content-item");

// Select tab content
function selectItem(e) {
  removeBorder();
  removeShow();
  // Add border to current tab
  this.classList.add("tab-border");
  // Grab content item from DOM
  const tabContentItem = document.querySelector(`#${this.id}-content`);
  // Add show class
  tabContentItem.classList.add("show");
}
function removeBorder() {
  tabItems.forEach(item => item.classList.remove("tab-border"));
}
function removeShow() {
  tabContentItems.forEach(item => item.classList.remove("show"));
}
// Listen for tab click
tabItems.forEach(item => item.addEventListener("click", selectItem));
```

And for the HTML All you really need is this:

```html
<!-- Content Pretty Long so I'll add later -->
<!-- But this is the basic gist -->
<div class="tab-item">
  <!-- Selectors for the different tab content -->
</div>
<div class="tab-content-item">
  <!-- Content of each tab item -->
</div>
<!-- Simply add more selectors and corresponding 
tab content for each selector -->
```


## Features in Development

I might add the other pages on the Netflix website if I ever come back to refactor ^-^


That being said
_<p align="center">To the Front... to the Back... End to End... cut no slack. Making ends meet. lol</p>_
