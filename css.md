# Top CSS Interview Questions | CSS Interview Questions And Answers | CSS Training

---

# BASIC && ADV

## Name some css frameworks?

- css Frameworks are libraries that make web page styling easier. Some of them are **foundation,Bootstrap,Styled-component,Ukit**

## What do understand by the universal selector?

- A universal selector is a selector that matchs any element typ's name instead of selecting elements of a particular type.

```
*{
    color:blue;
    font-size:10px;
}
```

## Tell us about the use of ruleset?

- The ruleset is used for the identification of selectors, which can be attached with other selector, the two parts of a rulset are: - Declaration Block:- Contains one or more semicolon-separated declarations. - Sector: Indicates the HTML element needed to be styled

# What does CSS stand for, and what is its primary purpose?

- CSS stands for Cascading Style Sheets and is used to style the layout and presentation of HTML documents.

# How do you link an external CSS file to an HTML document?

- To link an external CSS file to an HTML document, use the <link> tag in the HTML head section with the "rel" attribute set to "stylesheet" and the "href" attribute pointing to the CSS file's location.

#  Explain the difference between classes and IDs in CSS. When would you use one over the other?

- Classes are used to select multiple elements with the same styling, while IDs are used to select a unique element. Use classes for elements with shared styles and IDs for unique elements.

# How do you select all paragraphs on a web page using CSS?

- To select all paragraphs on a web page, use the "p" selector in CSS: p { /* styles here */ }.

# How can you center an element horizontally and vertically using CSS?

```
.centered-element {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
```

# What is the box model in CSS? Describe the components of the box model.

- The box model in CSS defines how elements are rendered in a rectangular box, consisting of content, padding, border, and margin.

# How do you set a background image for a specific element in CSS?

- To set a background image for an element, use the "background-image" property in CSS: background-image: url('image.jpg');.

# Explain the "float" property in CSS and how it affects the layout of elements.

- The "float" property in CSS is used to position elements to the left or right of their containing element, affecting the layout of subsequent elements.

# What is a media query, and how is it used in responsive web design?

- Media queries are used in responsive web design to apply CSS styles based on the user's device characteristics (e.g., screen size, resolution). Example: @media screen and (max-width: 768px) { /* styles here */ }.

# How do you create a simple CSS animation or transition?

- To create a simple CSS animation or transition, use the "animation" or "transition" properties with appropriate values for the desired effect.

# What are pseudo-classes in CSS? Provide an example of when you might use one.

- Pseudo-classes in CSS are used to select and style elements in specific states, such as :hover for when the user hovers over an element.

# Describe the difference between inline and block-level elements in CSS.

- Inline elements do not start on a new line and only take up as much width as necessary, while block-level elements start on a new line and take up the full available width.

# How do you hide an element in CSS while still keeping it accessible to screen readers?

- To hide an element while keeping it accessible to screen readers, use the following CSS: visibility: hidden; or opacity: 0;.

# How can you target and style elements based on their parent-child relationship using CSS?

- To target and style elements based on their parent-child relationship, use descendant selectors or child selectors in CSS.

# What is the purpose of CSS vendor prefixes, and can you provide an example of when to use them?

- CSS vendor prefixes are used to apply experimental or browser-specific CSS properties. Example: -webkit-border-radius. They are less commonly needed nowadays due to browser support improvements.






---
# Adv

What is CSS selector specificity and how does it work? <br>
What's the difference between "resetting" and "normalizing" CSS? Which would you choose, and why? <br>
Describe Floats and how they work. <br>
Describe z-index and how stacking context is formed. <br>
Describe BFC (Block Formatting Context) and how it works. <br>
What are the various clearing techniques and which is appropriate for what context? <br>
How would you approach fixing browser-specific styling issues? <br>
How do you serve your pages for feature-constrained browsers? <br>
What techniques/processes do you use? <br>
What are the different ways to visually hide content (and make it available only for screen readers)? <br>
Have you ever used a grid system, and if so, what do you prefer? <br>
Have you used or implemented media queries or mobile specific layouts/CSS? 
Are you familiar with styling SVG? <br>
Can you give an example of an @media property other than screen? <br>
What are some of the "gotchas" for writing efficient CSS? <br>
What are the advantages/disadvantages of using CSS preprocessors? <br>
Describe what you like and dislike about the CSS preprocessors you have used. <br>
How would you implement a web design comp that uses non-standard fonts? <br>
Explain how a browser determines what elements match a CSS selector.<br>
Describe pseudo-elements and discuss what they are used for. <br>
Explain your understanding of the box model and how you would tell the browser in CSS to render your layout in different box models. <br>
What does * { box-sizing: border-box; } do? What are its advantages? <br>
What is the CSS display property and can you give a few examples of its use? <br>
What's the difference between inline and inline-block? <br>
What's the difference between the "nth-of-type()" and "nth-child()" selectors? <br>
What's the difference between a relative, fixed, absolute and statically positioned element? <br>
What existing CSS frameworks have you used locally, or in production? How would you change/improve them? <br>
Have you used CSS Grid? <br>
Can you explain the difference between coding a web site to be responsive versus using a mobile-first strategy? <br>
Have you ever worked with retina graphics? If so, when and what techniques did you use? <br>
Is there any reason you'd want to use translate() instead of absolute positioning, or vice-versa? And why? <br>
How is clearfix css property useful? <br>
Can you explain the difference between px, em and rem as they relate to font sizing? <br>
Can you give an example of a pseudo class? Can you provide an example use case for a pseudo class? <br>
What is the difference between a block level element and an inline element. Can you provide examples of each type of element? <br>
What is the difference between CSS Grid and Flexbox? When would you use one over the other? <br>























