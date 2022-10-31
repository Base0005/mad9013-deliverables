# Grade

Use of variables: 0/1
Modifier class: .5/1
General CSS Code Quality: .5/1
Design Matching: 1/1
File Organization & Commits: 1/1
Total: 3/5

## Comments
The goal of this assignment was to set the banner height (`min-height`), vertical alignment (`align-items`), and horizontal alignment (`justify-content` and `text-align`) with variables and then update those variables with the modifier classes.

Checkout the explainer video for more information:
https://youtu.be/gHbZ92-kOK4

A couple specific comments:
- CSS variables were not used
- You should avoid setting large amount of margin with specific values like `25em` when attempting to adjust layouts. It is in-flexible and will cause numerous responsive issues.
  - You'd need to constantly update the margin values for the alignment to work for each slightly different screen size.
- NEVER set a specific `height` value. It will cause overflow issues for your content. Use `min-height` instead.
- All alignment/layout changes can accomplished with `min-height`, `align-items`, `justify-content` and `text-align`
