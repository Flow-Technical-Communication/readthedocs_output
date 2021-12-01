---
author: [Pieterjan Vandenweghe, Pieterjan.vandenwegh]
category: DITA
audience: 
---

# What is a DITA map?

A DITA map is a collection of topics assembled into a sequence and hierarchy.

## Description

DITA maps are files with the extension .ditamap. Unlike topics, DITA maps should not contain any content of their own. Instead, they contain references to the content and provide a structure for these references. In this sense, you can best compare a DITA map to an outline that describes the hierarchy and the order of its topics.

## Hierarchy and nesting

DITA maps contain the structure of your topic references. This structure resembles a table of contents and helps your reader locate the required information. To create a meaningful structure, you can group relevant topics together and nest them under a topic grouping or title-topic. The head topic is referred to as the 'parent topic' and the nested topics underneath it as its 'child topics'. The relationship between the child topics is defined as 'siblings'.

![](../_media/graphics/ditamap_hierarchy.png)

Here you can see the table-of-contents-like structure of a DITA map created by the nested topics:

![](../_media/graphics/dita_map_tree_structure.png)

**Related information**  


[Why use DITA maps?](co_why_use_ditamaps.md)

[What are the main components of a DITA map?](co_main_components_ditamap.md)

[To create a new DITA map](ta_to_create_a_ditamap.md)

[Guidelines for creating DITA maps and bookmaps](re_guidelines_ditamaps.md)

