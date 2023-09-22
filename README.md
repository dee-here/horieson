# Horiseon 

This project was to refactor Horiseon's website codebase, to make it follow accessibilty standards and for search engine optimization.


## Technology Used 

| Technology Used         | Resource URL           | 
| ------------- |-------------| 
| HTML    | [https://developer.mozilla.org/en-US/docs/Web/HTML](https://developer.mozilla.org/en-US/docs/Web/HTML) | 
| CSS     | [https://developer.mozilla.org/en-US/docs/Web/CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)      |   
| Git | [https://git-scm.com/](https://git-scm.com/)     |    


## Description 

[Horiseon website](https://dee-here.github.io/horieson/)

To make the code accessibility compliant and search engine optimized, these are some of the changes made: 
* Use more semantic elements like header, footer, nav, aside etc instead of generic div and spans.
* Images now have an accessible alt attribute.
* HTML elements follow a logical structure without styling and positioning.
* Heading attributes are sequential.
* Title element is concise and descriptive.


Other refactoring changes include:
* Fix broken link of Search Engine Optimization navigation text by adding the id to the specific article element.
* Renamed the generic "hero" class to more semantic class name.
* Make the classes more reusable. Instead of using three classes benefits-lead, benefits-brand and benefits-cost which have the exact same properties, used a less specific selector to target the same elements.



## Screenshots

<img src="./assets/images/horiseon-header-screenshot.png" height="200" >
<img src="./assets/images/horiseon-content-screenshot.png" height="200" >
<img src="./assets/images/horiseon-content-footer-screenshot.png" height="200" >


## Code Refactoring

Some code snippets to show the refactored changes:


```html
<div class="header">
        <h1>Hori<span class="seo">seo</span>n</h1>
        <div>
            <ul>
                <li>
                    <a href="#search-engine-optimization">Search Engine Optimization</a>
                </li>
                <li>
                    <a href="#online-reputation-management">Online Reputation Management</a>
                </li>
                <li>
                    <a href="#social-media-marketing">Social Media Marketing</a>
                </li>
            </ul>
        </div>
    </div>
```

header, and nav elements replaced divs.

```html
<header>
        <h1 title="Horiseon">Hori<span class="seo">seo</span>n</h1>
        <nav>
            <ul>
                <li>
                    <a href="#search-engine-optimization">Search Engine Optimization</a>
                </li>
                <li>
                    <a href="#online-reputation-management">Online Reputation Management</a>
                </li>
                <li>
                    <a href="#social-media-marketing">Social Media Marketing</a>
                </li>
            </ul>
        </nav>
    </header>

```

In style.css file, we removed class header and added style for the element header.

```css
.header {
    padding: 20px;
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
    background-color: #2a607c;
    color: #ffffff;
}
```
css for header element instead of header class.

```css
header {
    padding: 20px;
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
    background-color: #2a607c;
    color: #ffffff;
}

```


## Author Info

Deepak Sinha

* [Portfolio](https://dee-here.github.io/basic-landing-page/)
* [Github](https://github.com/dee-here)