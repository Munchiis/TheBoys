# The Boys

> Helpful links
<br> [MDN documentations](https://developer.mozilla.org/en-US/)
<br> [Google Fonts](fonts.google.com)

## **12/23/21 HTML BASICS** 

+ HTML = content/structure
+ CSS = Style
+ JS = Behavior/Interaction

```html
<p class = 'nice'> Hello World! </p>`
```

### **Heading Elements (tags)**

+ h1 through h6
  + choose tag based on importance and symantic reasoning
+ h1 is supposed to be most important content
  + typically used once

#### **other text elements**

```html
<p> paragraphs </p>
<span> Short text </span>
```

### **Container for elements**

```html
<div> general/common case </div>
<section> groups similar content </section>
<article> </article>
<aside> for side bars / ads </aside>
<header> beginning </header>
<footer> ending </footer>
```

### **Listing elements**
```html
<ul> unordered list where order does not matter</ul>
<ol> ordered list</ol>
<li> list items </li>
```
### **Anchor tags**
```html
<a> </a>
<a href= "#">  - use **href** for hyperlinks
```

### **Navigational Content**

```html
<nav> </nav> - usually inside of a header tag
```

___
## **CSS**
+ written in a separate file

    +   Add this inside of the `<head></head>`  tag to link css to html
        ```html
        <link rel="stylesheet" href="css/style.css">
        ```

rules can be parsed with selectors that are made of properties and values


> **CSS is read top to bottom**
<br> What comes below can override what came above

```css
p{
    color: blue;
}

p{
    color: red;
}
```

### CSS Colors

* Word
* Hex
* RGBa
* HSLa

```css
h1{color:red;}
h2{color:#FF00000;}
h3{color:rgba(255,0,0,1);}
h4{color:hsla(0,100%,50%,1);}
```

### CSS Font-family

```css
span{
    font-weight:700;
}
```

### CSS Relationship selectors

```html
<section>
    <p> </p>
</section>
```
#### relationships
```css
/*direct Parent -> child*/
section > p { /* '>' = only go one level deep || direct child/level deep */
    color: purple;
}

/* parent child*/
section p { /* all level deep */
    color:red;
}

/* sibling
* to select elements that is the next sibling  (Same level)
* only affects the NEXT sibling  
*/
p + p {
    color:blue;
}
```

### **Classes and IDs**

#### IDs are used for selecting distinct elements

`only one id with the same value per document` 
> `#id`

#### Classes are for selecting multiple elements 

`multiple with same value allowed per document`
> `.className`

```css
#id {
    color:blue;
}

.className{
    color:red;
}

p.className1.className2 { 
    /* no spaces between classes means only affects target <p></p> with all classes named */
    color:orange;    
}
```

# The Box Model
