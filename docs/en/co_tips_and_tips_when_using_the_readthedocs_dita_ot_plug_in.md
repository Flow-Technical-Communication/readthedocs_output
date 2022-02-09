---
author: [Pieterjan Vandenweghe, Pieterjan Vandenweghe]
keyword: 
---

# Tips and tips when using the ReadtheDocs DITA-OT plug-in

## Home page

The plug-in creates a home page for your static site based on a DITA topic. This can be:

-   The first topic in your DITAMAP or BOOKMAP file.
-   The topic added as `bookabstract` in your BOOKMAP file.

## Different blocks

Make use of the `topichead` element to create different blocks in the project. Title only topics lead to corrupt YAML configuration files.

## Levels of indentation

Do not use to many levels of indent in your project. Static sites in general do not use a lot of indented levels after being divided in blocks. Consider using the `@chunk` attribute to get more information on one page.

