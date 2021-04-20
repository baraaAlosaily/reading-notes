# CSS layout

![p](https://bs-uploads.toptal.io/blackfish-uploads/uploaded_file/file/197751/image-1583189914017-454f3b1dafc1fe0b0f3b35ec33aecf39.png)

For starters, here’s the HTML5 markup we’ll use with our sample implementation using classic CSS:

```
<body class="layout-classic">
  <header id="header"></header>
  <nav id="nav"></nav>
  <aside id="subnav"></aside>
  <main id="main"></main>
  <footer id="footer"></footer>
</body>
```

## Use Case

One of the best ways to learn a technology is to have a specific use case you’re attempting to support or a particular problem you’re trying to solve. Toward that end, we’ll focus on a use case with a specific set of requirements.

Our use case consists of a Web App layout with some dynamic behavior. It will have fixed elements on the page such as a header, footer, navigation menu and sub-navigation, as well as a scrollable content section. Here are the specific layout requirements:

1. Basic Layout
   Header, footer, navigation menu, and sub-navigation all remain fixed on scroll
   Navigation and sub-navigation elements occupy all vertical free space
   Content section uses all remaining free space on the page and has a scrollable area
2. Dynamic Behavior
   Navigation menu only shows icons by default, but can be expanded to display text as well (and can then be collapsed to again show only icons)
3. Layout Variations
   Some pages have sub-navigation next to the navigation menu and some do not

### Fixed Positioning

In CSS, we can achieve the fixed elements on the page (header, footer, etc.) by employing a positioned layout model that uses fixed positioning.

In addition, we’ll use the z-index CSS property to ensure that our fixed elements remain “on top of” the other content on the page. The z-index property specifies the stack order of an element, where an element with greater stack order is always “on top of” an element with a lower stack order. Note that the z-index property only works with positioned elements. For our example, we’ll arbitrarily use a z-index value of 20 (which is higher than the default) to ensure that our fixed elements remain visually at the forefront.

Also, we’ll set the width property to 100% which instructs the browser to use all available space horizontally for the element.

```
#header, #footer {
  position: fixed;
  width: 100%;
  z-index: 20;
}

#header {
  top: 0;
  height: 5em;
}

#footer {
  bottom: 0;
  height: 3em;
}
```

### CSS Expansion

For the #nav and` #subnav`, we’ll use a slightly more sophisticated technique known as CSS Expansion, which can be used when positioning elements as fixed (i.e., at a fixed position on the page) or as absolute (i.e., at a specified position relative to its closest positioned ancestor or to the containing block).

Vertical expansion is achieved by setting both the top and bottom properties of an element to a fixed value, so the element will expand vertically to use the remaining vertical space accordingly. Basically what you’re doing is tying the top of the element to a specific distance from the top of the page and the bottom of the element to a specific distance from the bottom of the page, so the element expands to fill the entire vertical space between those two points.

Similarly, horizontal expansion is achieved by setting both the left and right properties of an element to a fixed value, so the element will expand horizontally to use the remaining horizontal space accordingly.

For our use case, we need to use vertical expansion.

```
#nav, #subnav {
  position: fixed;
  top: 6em;     /* leave 1em margin below header */
  bottom: 4em;  /* leave 1em margin above footer */
  z-index: 20;
}

#nav {
  left: 0;
  width: 5em;
}

#subnav {
  left: 6em;    /* leave 1em margin to right of nav */
  width: 13em;
}
```

### Default (Static) Positioning

The main scrollable content area can simply rely on default (static) positioning, whereby elements render in order as they appear in the document flow. Since everything else on our page is in a fixed position, this element is the only one that is in the document flow. As a result, all we need to do to position it properly is to specify its margin property to avoid any overlap with the fixed header, footer, and `nav/subnav:`

```
#main {
  margin: 6em 0 4em 20em;
}
And with that, we’ve satisfied the basic layout requirements of our use case using CSS2, but we still need to satisfy the additional requirements for dynamic functionality
```

### Summary

1. `<div>` elements are often used as containing elements to group together sections of a page.
2. Browsers display pages in normal flow unless you specify relative, absolute, or fixed positioning.
3. The float property moves content to the left or right of the page and can be used to create multi-column layouts. (Floated items require a defined width.)
4. Pages can be fixed width or liquid (stretchy) layouts.
5. Designers keep pages within 960-1000 pixels wide, and indicate what the site is about within the top 600 pixels (to demonstrate its relevance without scrolling).
6. Grids help create professional and flexible designs.
7. CSS Frameworks provide rules for common tasks.
8. You can include multiple CSS files in one page.
