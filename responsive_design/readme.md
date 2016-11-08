# CSS Responsive Design Exercise

### Part I

Answer the following questions

- What is an `em`? **An em is a unit for measuring and is relative to the font-size of the parent element. If the font size of the parent element was 16px, 2em would be equivalent to 32px**
- What is the difference between `em` and `rem`? **em is relative to a parent element and rem is relative to the root element**
- What is "mobile first" design? **mobile first design is the idea of first designing and building interfaces for mobile and then expanding to larger screen sizes as opposed to the opposite.**
- What is BEM? **BEM — Block Element Modifier is a methodology around naming and structure css and front-end code. When working with lots of other developers, it becomes very difficult to standardize around the naming of classes and structure of CSS. BEM aims to help with these issues.**

### Part II

For this exercise you will be building a small grid system! Your task is to create the following classes:

`.col-4` -  consumes 33% of the width when the screen size is greater than 960 pixels, 50% of the width when the screen size is greater than 765 pixels and 100% of the width when the screen size is less than 765 pixels.

`.col-6` -  consumes 50% of the width when the screen size is greater than 960 pixels and 100% of the width when the screen size is less than 960 pixels

`.col-12` - consumes 100% of the width when the screen size at all sizes.


```css
.col-4 {
    width: 33%;
}

.col-6 {
    width: 50%;
}

.col-12 {
    width: 100%;
}

@media (min-width: 765px) and (max-width: 960px){
    .col-4 {
        width: 50%;
    }

    .col-6 {
        width: 100%;
    }
}

@media (max-width: 765px){
    .col-4 {
        width: 100%;
    }
}
```

