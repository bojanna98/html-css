# Naming Conventions (HTML & CSS)
## HTML Naming Conventions
## Class and ID Names 
- When giving an element an id or class, give it a descriptive name, such as main-heading or announcements.
- Avoid one-letter names like x or c.

## Letter-Casing and Special Characters 
- Always favor lowercase, for elements, for attributes and their values, for classes and ids. Multi-word names for classes and ids should either 1., concatenate the words in lowercase without any in-between character, or 2., separate each word with a "-" (not "_") and maintain lowercasing throughout. Regardless of whether you prefer convention 1. or convention 2., you should not switch between the two conventions (remember, consistency is key in web programming). No other special characters should be used for separating words, and there should never be capitalization of the next word.

**BAD EXAMPLE**

`<h1 id="first_heading"></h1>`

`<p Class="importantReminder"></p>`

**GOOD EXAMPLE**

`<h1 id="mainheading"></h1>`

`<p class="importantreminder"></p>`

`<h1 id="main-heading"></h1>`

`<p class="important-reminder"></p>`

## CSS Naming Conventions
The following are naming conventions that you can employ:
- BEM
- SMACSS
- ITCSS
- OOCSS
- AMCSS
> BEM

BEM stands for *Block Element Modifier*. The idea behind BEM is to divide the *user interface* into independent blocks.
### What is a block?
- In BEM a block is an independent page component that can be reused represented by class attribute in HTML. The block name should describe *its purpose* **not what the element looks like nor how it behaves.**
### What is an element?
- An element is a composite part of a block that can't be used separately from it. You can think of an element like a mother—child relationship. The element name is separated from the block with a double underscore (__).
### What is a modifier?
- A BEM modifier defines the appearance, state or behavior of a block element. The modifier name is separated from the block or element name by a single underscore (_) and it **can not be used alone.**
>SMACSS

SMACSS stands for *Scalable and Modular Architecture for CSS.*
- SMACSS is about categorizing CSS rules into 5:

1. Base
2. Layout
3. Module
4. State
5. Theme
 ### Base rules
- Base rules are the defaults and they can include attribute selectors, pseudo-class selectors, child selectors or sibling selectors.
### Layout rules
- Layout rules divide the page into sections e.g header, footer e.t.c
### Module rules
- Modules are the reusable modular part of design. They can include:
   - navigation bars
   - dialog boxes
### State rules
-    State rules are ways to describe how the modules or layouts will look like when in a particular state. A state can be any of the following:
   - collapsed
   - expanded 
   - disabled
### Theme rules
- Theme rules are similar to state rules in that they describe how modules or layouts might look.
> ITCSS

ITCSS stands for *Inverted Triangle CSS* and its main philosophy is to help you organize your project CSS files in such a way that you can better deal the cascade, selectors and specificity.
> OOCSS

OOCSS means Object Oriented CSS and its purpose is to encourage code reuse and ultimately stylesheets that are easier to maintain. OOCSS is centered around two main principles:
- Separation of structure from skin
- Separation of container and content
> AMCSS

AMCSS is short for *Attribute Module for CSS* and the whole idea is about using HTML attributes and their values rather than classes for styling elements.