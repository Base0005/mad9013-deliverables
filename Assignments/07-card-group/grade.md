# Grade

HTML Code Quality: .5/1
CSS Code Quality: 1/2
Design Matching: .75/1
File Organization & Commits: 1/1
Total: 3.25/5

## Comments

### HTML
- There should be a `<section>` around all of the content as this is a section of related content.
- We are assuming this pattern is part of a bigger web page, therefore the `<h1 class="card__group">` should be an `h2` as it likely would not be the main heading on the page.
  - Because of the change from h1 --> h2, we would also need to update the `<h2 class="card__title">` to `h3`
- `<button class="card__btn">` should be `<a class="card__btn" href="#">`. These cards presumably link to another page, therefore we should be using an anchor.


### CSS
- Do not use `px` units. They are absolute units and cause accessibility issues.
  - User `rem` instead.
- Use `1fr` instead of `auto`. For example: `grid-template-columns: 1fr 1fr 1fr;`. `auto` will set the column to the width of the column content, whereas `1fr` will set the columns equal to each other (all the same size in the example).
  - In this example, `auto` is working because all of the content is the same size, but you could run into issue if the content is different.
- You should be re-using styles from previous assignments to simplify things. You should have included `.container`, `.btn`, and Type Hierarchy styles.
- Put the green background color on the `section` and add some padding on the top and bottom. Remember, we are assuming this is a pattern that is going to be included in other areas of our site, so we should have it all self contained.