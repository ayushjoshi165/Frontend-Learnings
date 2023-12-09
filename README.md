# Frontend-Learnings

##CSS
### Specificity and Selectors 

Specificity is used to decide the precedence of css whic h will be applied 
Example :
- Specificity of Inline style is 1000
- Specificity of id is 100
- Specificity of Class, pseudo class, Attribute selectors is 10
```
.myClass {
  font-size: 16px;
}

input[type="text"] {
  border: 1px solid #ccc;
}
```

- Specificity of Element, pseudo element is 1

```
p {
  font-weight: bold;
}

p::first-line {
  color: green;
}
```
### pseudo Classes and Pseudo Elements 

- Pseudo-classes:
Pseudo-classes are used to select elements based on their state or position. They are preceded by a colon (:) and are applied to existing selectors. Here are a few examples:

1. :hover
css
```
a:hover {
  color: red; /* Styles applied when the link is hovered over */
}   ```

```
2. :focus
css
```
input:focus {
  border: 2px solid blue; /* Styles applied when the input is focused */
}   ```

```
3. :nth-child
css

```

li:nth-child(odd) {
  background-color: lightgray; /* Styles applied to odd list items */
}   ```

```
- Pseudo-elements:
Pseudo-elements, on the other hand, allow you to style specific parts of an element. They are also preceded by a double colon (::). Here are some examples:

1. ::before
css
```
p::before {
  content: "★"; /* Adds a star before each paragraph */
}   ```
2. ::after
css
```
p::after {
  content: " - The end"; /* Adds content after each paragraph */
}   ```
```
3. ::first-line
css
```
p::first-line {
  font-weight: bold; /* Styles the first line of each paragraph */
}   ```
```
4. ::first-letter
css
```
p::first-letter {
  font-size: 150%; /* Styles the first letter of each paragraph */
}   ```
```
Pseudo-elements are used to style parts of elements that don't correspond to a real HTML element. They are commonly used to add decorative elements or to style the first letter/line of a block of text.

Here's a quick example combining both pseudo-classes and pseudo-elements:

css
```
button:hover::before {
  content: "🚀"; /* Adds a rocket emoji before the button text on hover */
}   ```
```
In this example, the ::before pseudo-element is applied only when the button is hovered over.

## Selectors in CSS

Selectors in CSS are patterns that are used to select and style HTML elements. They define the elements to which a set of CSS rules should be applied. Selectors can be simple, targeting specific elements, or complex, allowing for more fine-grained control over styling.

Here are some common types of selectors:

Type Selector:

Selects all instances of a specified HTML element.
css
```
p {
  color: blue;
}   ```
Class Selector:

Selects all elements with a specific class attribute.
css
```
.highlight {
  background-color: yellow;
}   ```
ID Selector:

Selects a single element with a specific id attribute.
css
```
#header {
  font-size: 24px;
}   ```
Descendant Selector:

Selects an element that is a descendant of another specified element.
css
```
article p {
  font-style: italic;
}   ```
Child Selector:

Selects an element that is a direct child of another specified element.
css
```
ul > li {
  list-style-type: square;
}   ```
Adjacent Sibling Selector:

Selects an element that is directly preceded by a specified element.
css
```
h2 + p {
  font-weight: bold;
}   ```
Attribute Selector:

Selects elements based on the presence or value of their attributes.
css
```
input[type="text"] {
  border: 1px solid #ccc;
}   ```
Pseudo-class Selector:

Selects elements based on their state or position.
css
```
a:hover {
  color: red;
}   ```
Pseudo-element Selector:

Selects a specific part of an element.
css
```
p::first-line {
  font-weight: bold;
}   ```
These selectors can also be combined for more complex selections. For example:

css
```
ul.nav > li.active a {
  color: red;
}   ```
This selector targets an <a> element that is a child of an <li> element with the class "active," which in turn is a child of a <ul> element with the class "nav."

