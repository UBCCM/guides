# CSS

* [Methodologies](#methodologies)
* [Structure](#structure)
* [Selector](#selector)
* [Properties](#properties)
* [Declaration Order](#declaration-order)
* [Vendor Prefixes](#vendor-prefixes)

# Methodologies
## BEM
Use of BEM methodology to collaborate on large CSS code base in a maintainable manner.
* [Detail on BEM](http://getbem.com/introduction/)

# Structure
* Each selector should be on its own line, ending in either a comma or an opening curly brace.
* Each declaration should be indented one level relative to its selector with an ending semicolon.

Example:
```css
.selector-alpha,
.selector-beta {
    counter-reset: section;
    text-transform: small-caps;
}
```

# Selector
* Use lowercase and separate words with hyphens and underscore when naming selectors.
* Use snake case (Not camelCase)

Correct:
```css
.class-name {
    color: #ffffff;
}
```
Incorrect:
```css
.className {
    color: #ffffff;
}
```
# Properties
* Property name should be immediately followed by a colon, then a single space, and then the property’s value.
* Use lowercase, including hex color: `#aaa`
* For property values that require quotes, use double quotes instead of single quotes
* Avoid specifying units for zero-values.

# Declaration Order
* The declarations in a ruleset should be ordered so that the purpose of the declaration block is most obvious. 
1. Display
2. Positioning: `position, float, clear, top, right, bottom, left, direction, and z-index`
3. Box model: `[(max|min)-]height, [(max|min)-]width, margin, padding, border, box-sizing`
4. Colors and Typography
5. Other

# Vendor Prefixes
* Should be avoid adding them manually and generate them through autoprefixer through pre-processor tool, gulp or grunt.