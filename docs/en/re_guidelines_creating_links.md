---
author: Pieterjan Vandenweghe
category: DITA
---

# Guidelines for creating links

## Do not over-use inline links

It is easy to over-use inline links in your text, rendering it confusing to the reader. It is important to use them only when necessary and keep in mind the following guidelines:

-   Avoid inline links to tables and figures in a topic.

    This should be avoided as you should keep your topics short and self-contained. These links can become difficult to maintain when you update your topics, for instance by deleting a table or moving it to a different topic. They can also make it difficult to re-use topics. Instead, you can consider re-using the table or the figure somewhere else in the form of a content reference.

-   Create inline links to repeated steps

    You might use phrases such as 'Repeat step 2 to add each topic to the DITA map'. In this case you will need to update this phrase every time you add a step before 'step 2'. You can solve this by adding an `xref` element that links to the relevant step. In doing so, every time the numbering changes in the steps, the `xref` element will ensure the text changes automatically.

-   Create inline links to high-level tasks.

    If you have a manual that contains a task flow with 10 different task topics for installation, another 15 task topics for post-installation configuration and yet another set of tasks for setting up security, the user might start to lose track of the big picture. As these tasks might be spread throughout your DITA map, it can happen you can't take advantage of the default linking system. In this case, you can use inline links to show users a roadmap of the task flow they will have to follow. This way, they can plan for tasks they will need to complete in the future.


## Think about the phrasing and positioning of inline links

For all their advantages, inline links are not without flaws. Tests conducted by user experience specialist Jared Spool support the view that links outside of the text are more effective than inline, embedded links. He concluded that:

-   Links are less usable when embedded in the text.
-   Longer links are more effective than shorter ones.
-   People scan for target words - the scent of information.

## Do not over-use relationship tables

Relationship tables are useful in linking content that does not get linked by the hierarchical linking system. Still, it is important not to link too much. What applies for inline linking, applies for relationship tables as well. Too many links will merely confuse the user.

A good general rule to keep in mind is that hierarchical linking is nearly error-proof and low maintenance. As such, it is a good system to rely on. Only start adding relationship tables if you require relevant topics of information to be linked for the user's convenience. When you do, follow these guidelines:

-   Add links for sibling topics if you set the `@linking` attribute to none in the parent topic but want to have related links for a select few of the child topics.
-   Add links between topics that would not otherwise be there in the hierarchy of links.
-   Add links to topics outside of the hierarchy in the current DITA map.
-   Keep the number of related links in each topic to fewer than five when possible.

## Add collection-type links

A collection type defines a relationship among nested topics and affects the way in which automatic links are generated in the output of your DITA map. The `@collection-type` defines the type of hierarchical relationship between members of the same branch of a ditamap tree, or in the same cell in the relationship table relcell element.

**Parent topic:**[Guidelines for writing in Oxygen XML](../en/to_guidelines_and_tips_oxygen_xml.md)

**Related information**  


[Why create links?](co_why_create_links.md)

[What does collection-type do?](co_collection_type.md)

