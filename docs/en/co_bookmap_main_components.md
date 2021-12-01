---
author: Pieterjan Vandenweghe
category: DITA
audience: 
---

# What are the main components of a bookmap?

## Component list

Bookmaps \(`bookmap`\) contain components which are similar to the parts of a traditional book. The topic references therefore are labeled according to the book components they represent. A bookmap can contain:

|Component|Purpose|
|---------|-------|
|`booktitle`|Contains the title information for a book. See .[What are the main components of a bookmap?](co_bookmap_main_components.md)|
|`bookmeta`|Contains copyright information, author information and publishing data. See [Bookmap metadata](co_including_metadata.md).|
|`frontmatter`|Contains cover, table of contents, booklists, details of production, dedication for a person or group, introduction to the draft of the book, preface and a bookabstract. See [What are the main components of a bookmap?](co_bookmap_main_components.md)|
|`chapter`|Groups topic references. See .[What are the main components of a bookmap?](co_bookmap_main_components.md)|
|`part`|Divides chapters into logical groups. See .[What are the main components of a bookmap?](co_bookmap_main_components.md)|
|`appendix`|Contains notices and dedications. [What are the main components of a bookmap?](co_bookmap_main_components.md).|
|`backmatter`|Contains legal notices, booklists, details of production and updates. See [What are the main components of a bookmap?](co_bookmap_main_components.md).|
|`reltable`|Specifies relationships between topics, linking them outside of the relationships defined by the hierarchy. See [To create a relationship table](ta_to_create_a_reltable.md).|
|`booklists`|References lists of various kinds within the book. See [What are the main components of a bookmap?](co_bookmap_main_components.md).|

**Note:** A bookmap should contain no content, but also no direct topic references. Instead, bookmaps should contain only DITA map references which, in turn, can contain topic references. These DITA maps are then the chapters or parts of your book.

## Example

The image below lists the possible main components of a DITA bookmap:

![](../_media/graphics/bookmap_example.png)

**Related information**  


[What is a bookmap?](co_what_is_a_bookmap.md)

[Why use bookmaps?](co_why_use_bookmaps.md)

[To create a new DITA bookmap](ta_to_create_a_bookmap.md)

[What are the main components of a DITA map?](co_main_components_ditamap.md)

