# em and rem Units:
 - Both em and rem are units of measurement in CSS that are used to define sizes in a relative manner.

em:

The em unit is relative to the font-size of its closest parent or the element itself.

For example, if the font-size of an element is 16px, 1em is equal to 16px, and 2em is equal to 32px.

It can be used for various properties, not just font-size.

css
```
.parent {
  font-size: 16px;
}

.child {
  font-size: 1.5em; /* 1.5 times the font-size of the parent, so 24px */
}
```
rem (root em):

The rem unit is relative to the font-size of the root element (usually the <html> element).

This makes rem particularly useful for creating consistent sizing across the entire document.

```
html {
  font-size: 16px;
}

.child {
  font-size: 2rem; /* 2 times the root font-size, so 32px */
}

```
