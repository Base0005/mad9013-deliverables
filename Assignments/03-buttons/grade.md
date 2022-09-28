# Grade

HTML Code Quality: .75/1
CSS Code Quality: 1.25/2
Design Matching: 1/1
File Organization & Commits: 1/1
Total: 4/5

## Comments
Overall great, you've got the concept of base class with modifiers down which was the goal. Just a few small things:
- File and folder names should be all lowercase
- Do not put `<button>` inside of `<a>`. We are applying to style through the class `.btn` and one of the points of the lesson was to demonstrate how we can set up our styles to work on different tags. Meaning the styles should look exactly the same on both of these elements: `<button class="btn btn--Primary">Primary</button>` and `<a class="btn btn--Primary">Primary</a>`
- Do not use `px` units. They are absolute units and cause accessibility issues.
- Use `em` for `padding` and `border-radius` unit size. This will allow the `padding` to grow/shrink based on the size of the text. If you do so, you don't need to change the `padding` on the small/large buttons;
- Include `cursor: pointer;` on the `.btn` class to show the hand pointer mouse when interacting with the button.
- You should include both a `:hover` and a `:focus`