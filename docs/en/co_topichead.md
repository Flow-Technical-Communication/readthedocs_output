---
keyword: [topicgroup, topicmeta, topicset]
---

# Map structure elements

To structure the map, you can nest `topicref` elements, but this creates a structural hierarchy as well. Therefore, you can use the `topicgroup` element to group `topicref` elements without affecting the hierarchy of the map. The elements does not affect navigation or the table of contents, but it links the elements it contains and provides shared, inherited attributes.

Furthermore, the `topicmeta` element:

-   Defines the metadata for a topic and all its children
-   Optionally, overrides the `title` and `shortdesc` that are used for links
-   Optionally, adds index entries to referenced content using the `keywords` element

**Note:** Text in metadata cannot be seen by the reader, only by the writer.

When writing a larger task which consists of multiple smaller tasks, the `topicset` element can help define a complete unit of content \(containing all smaller tasks\) that can be reused in other DITA maps or other `topicset` elements.

**Note:** To ensure the complete unit is available for reuse, the `@id` attribute is mandatory.

**Related information**  


[What is a DITA map?](co_what_is_a_ditamap.md)

[What are the main components of a DITA map?](co_main_components_ditamap.md)

[Map elements](co_creating_map.md)

