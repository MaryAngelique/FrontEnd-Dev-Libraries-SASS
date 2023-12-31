Sass allows nesting of CSS rules, which is a useful way of organizing a style sheet.

Normally, each element is targeted on a different line to style it, like so:

nav {
    background-color: red;
}

nav ul {
    list-style: none;
}

nav ul li {
  display: inline-block;
}
For a large project, the CSS file will have many lines and rules. This is where nesting can help organize your code by placing child style rules within the respective parent elements:

nav {
    background-color: red;

    ul {
        list-style: none;

        li {
        display: inline-block;
        }
    }
}

Use the nesting technique shown above to re-organize the CSS rules for both children of .blog-post element. For testing purposes, the h1 should come before the p element.


Tests
Your code should re-organize the CSS rules so the h1 and p are nested in the .blog-post parent element.