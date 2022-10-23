# Grade

HTML Code Quality: .75/1
CSS Code Quality: 1.25/2
Design Matching: 1/1
File Organization & Commits: 1/1
Total: 4/5

## Comments
Overall great! A couple things:
- You should include a real descriptive `<title>` in the `<head>`.
- The logo should have an `<h1>` in it on the home page.
- The default `.container` class should have `margin: 0 auto;` and `padding-left: 1.5rem;` and `padding-right: 1.5rem;`
  - This sets up the consistent styles we need across our site.
  - If you need to remove some of those styles in the navbar, remove the styles in the `.header .container`
- Put the hover state & styles (with the background color) on the `.header ul a` not on `li`. A change in state like that suggests that that element is clickable. However, in your version you can only click on the actual text of the link, not the entire hover-able element. This creates a poor user experience. It is also not possible to `focus` on the `li` by default, instead you `focus` on the `a`, meaning the styles wouldn't work correctly for tabbing.
 - You need to make the `a` full width and add padding.
