# Topic 2 - CSS

## Description

Cascading Stylesheets — or CSS — is the first technology you should start learning after HTML. While HTML is used to define the structure and semantics of your content, CSS is used to style it and lay it out. For example, you can use CSS to alter the font, color, size, and spacing of your content, split it into multiple columns, or add animations and other decorative features.

## Index

1. [Selectors and properties](#selectors-and-properties)
2. [Specifity](#specificity)
3. [Box model](#box-model)
4. [Layout](#layout)

## Exercises

For this and the next exercises use the base template called index.html inside the assets. [here](../assets/index.html).

### Selectors and properties

#### Documentation

- [Introduction to CSS](https://developer.mozilla.org/en-US/docs/Learn/CSS)
- [Selectors](https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS/Selectors)
- [CSS3 selectors sheet](https://www.w3.org/TR/selectors-3/)
- [Reset style](https://meyerweb.com/eric/tools/css/reset/)
- [Normalize](http://necolas.github.io/normalize.css/)

1.A
- Learn why is a best-practice to use a reset stylesheet. Then, include the "normalize.css".
- Add background to the header, footer, aside and nav.
- Add a global font definition (at html element) with a value of 14px, using a font-family you like.
- Center the header and footer text.

### Specificity

#### Documentation

- [Cascade and inheritance](https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS/Cascade_and_inheritance#Specificity)

2.A

Add the following classes to the template created in the exercies 1.

- To ```<header>``` add class .header
- To ```<footer>``` add class .footer
- To ```<section>``` add class .content
- To ```<nav>``` add class .navigation
- To ```<aside>``` add class .sidebar

2.B

Using the new added classes figure out how to override.

- .header must have a font size of 46px
- .footer must have a font size of 10px
- .content must have a font size of 14px
- .navigation must have a font size of 12px
- .sidebar must have a font size of 10px

2.C

Add the following rules the previous css created.

- If the class attribute finishes with r (example header, footer), the background must be magenta.
- How could you add weight to the global font definition to win over the classes added by point 3?
- Imagine there is a declaration like class=”oh-no-inline-styles” style=”background:red” and you need to change the background to green without changing the inline style. How could you accomplish this?

### Box model

#### Documentation

- [Introduction to box model](https://developer.mozilla.org/en-US/docs/Learn/CSS/Styling_boxes/Box_model_recap)
- [Box model calculation](http://www.w3.org/TR/CSS21/box.html)
- [Other types of boxes](https://developer.mozilla.org/en-US/docs/Learn/CSS/Styling_boxes/Box_model_recap#Box_display_types)

3.A
- Use the playground provided above to change box-sizing
- Add padding of 140px to `.navigation`
- Add margin of 100px to `.sidebar`
- Experiment with the box-model [here](http://dabblet.com/gist/2986528) by changing width / margin / padding / box-sizing

### Layout

#### Documentation

- [Display property - part 1](http://learnlayout.com/display.html)
- [Display property - part 2](http://adamschwartz.co/magic-of-css/chapters/2-layout/)
- [Learn media queries](http://css-tricks.com/css-media-queries/)
- [Grid Systems](http://www.adamkaplan.me/grid/)
- [CSS Floats](http://alistapart.com/article/css-floats-101)
- [CSS units](http://alistapart.com/article/love-the-boring-bits-of-css)

4.A

- Modify your CSS to reach something similar to this layout:

![](https://raw.githubusercontent.com/globant-ui/css-lab/master/images/html5-structure.png)

4.B

- Investigate about _layout systems_
- Using your own layout system, implement an image gallery based on this `mock up`:
![](https://raw.githubusercontent.com/globant-ui/css-lab/master/images/example-layout.png?s=300)
- Adapt your the template system to work on three different breakpoints.

[<- To index](../README.md#title) - [Topic 3 - Javascript ->](./topic3.md)
