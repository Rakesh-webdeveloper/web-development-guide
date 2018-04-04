## Scalable and Modular Architecture for CSS
_A flexible guide to developing sites small and large._

There are five types of categories:
- Base
>Base rules are the defaults. They are almost exclusively single element selectors but it could include attribute selectors, pseudo-class selectors, child selectors or sibling selectors.
- Layout
>Layout rules divide the page into sections. Layouts hold one or more modules together.
- Module
>Modules are the reusable, modular parts of our design. They are the callouts, the sidebar sections, the product lists and so on.
- State
>State rules are ways to describe how our modules or layouts will look when in a particular state. Is it hidden or expanded? Is it active or inactive?
- Theme
>Theme rules are similar to state rules in that they describe how modules or layouts might look.
Divide the CSS into 5 category

---
Naming Rules

Base Rules
A Base rule is applied to an element using an element selector, a descendent selector, or a child selector, along with any pseudo-classes. It doesn’t include any class or ID selectors. It is defining the default styling for how that element should look in all occurrences on the page.  
**Example Base Styles**
```CSS
body, form {
    margin: 0;
    padding: 0;
}

a {
    color: #039;
}

a:hover {
    color: #03F;    
}
```
Base styles include setting heading sizes, default link styles, default font styles, and body backgrounds. There should be no need to use !important in a Base style.

### CSS Reset
A CSS Reset is a set of Base styles designed to strip out—or reset—the default margin, padding, and other properties. Its purpose is to define a consistent foundation across browsers to build the site on.
