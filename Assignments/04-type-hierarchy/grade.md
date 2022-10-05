# Grade

HTML Code Quality: .5/1
CSS Code Quality: .5/2
Design Matching: .5/1
File Organization & Commits: 1/1
Total: 2.5/5

## Comments
You need to spend time reviewing what we covered in class. You did not use the methods that I covered or creating a type hierarchy and style sheet.

Below are some of the major issues that need to be fixed. Please make sure to look at what we did and recreate it for the proper type hierarchy design for the project.

- You have not included a link to the font in your `html` nor included the font files with an `@font-face`. Because of this, the Roboto font is not loading and the back up font is being shown.
- `<title>Document</title>` --> include a real descriptive title.
- `<p class="h5">Heading 5</p>` should be `<h5>Heading 5</h5>`
- `<p class="h6">HEADING 5</p>` should be `<h6>Heading 6</h6>`
- You should not have any classes on the headings or anchor. We want to set all of these styles directly on the tag selectors (`h1`, `h2`, `a`, etc.) because they are the default styles and should not require using a class to apply.
- Do not type in all caps in `html`. A screen reader will think it is an acronym and read it out by letter. Use `text-transform` in css to make it uppercase.
- Do not use `px` units. They are absolute units and cause accessibility issues.
- You should be using the `type-scale.com` tool to generate the type scales. The type should be responsive and the scale should be set on the default size, then increased at the medium and large media query. Here are the sizes you should be using.
  - Default/Small: 1.125 (Major Second)
  - Medium: 1.2 (Minor Third)
  - Large: 1.25 (Major Third)
- `margin-bottom: 0%;` when the value is `0` you do not need to include a unit.
- Please review the `.container` styles covered in class. I provided the proper styles that should be used including proper width/max-width, margin, and padding values.
  - `font-family` should not be applied on the `.container`