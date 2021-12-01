---
author: [Pieterjan Vandenweghe, Pieterjan Vandenweghe]
category: [DITA, DITA]
audience: 
---

# Guidelines for using content references

Content referencing can cause a number of problems, so it is good to keep the following best-practices in mind:

## Do not adjust conrefs outside of their tags

At times, it can be very tempting to adjust your conref in its surrounding text, rather than making an entirely new conref. A common example of this is pluralizing nouns by adding an 's' outside of the tags: <keyword\>server</keyword\>s. While this can be a very easy solution that works in English, problems will start arising during translation. Every language has its own grammar and very often words change according to their context - something conrefs are not designed for. If you really need a pluralized form of a conref, it is best to just make a new one to suit the new context.

## Avoid conreffing single words and phrases

When a DITA file is entered into a translation program, problems can arise while translating conrefs. Conrefs get processed as tags and appear as such in the text to be translated. This means that the text they reference is not displayed; at best, the translator only gets to see the reference-ID. The original text is only visible in the topic you have referenced it from. This leads to two main context-related problems:

-   Without the original text available, it is impossible for the translator to know which word or phrase is being conreffed, making it difficult to translate the rest of the text correctly.
-   The translation of the conref in its original position might not make sense in its new context. Words can change their form depending on their context, but as the conref can only be changed once, the translation cannot be adapted to each of these new contexts.

As such, it is recommended you only conref full sentences and reserve the shorter conrefs for content you know is not affected by context, such as product names, menu cascades, filepaths and similar items.

## Do not make too many references

Conrefs are very useful if they are used sparingly for content that changes often, such as for product names or model numbers. Avoid using them for any sentence that is regularly used. Too many conrefs will only confuse you and your writers.

At times people are tempted to use conrefs for every repeated sentence so they can reduce translation costs. However, translation tools these days are mostly based on the concept of repeated content. They are designed to detect whether input has already been translated in the past and calculates to what extent the new input is similar to its database. As such, fewer new content needs to be translated and translation costs are automatically reduced.

## Do not nest conrefs

Theoretically, you can conref a productname inside a paragraph that you then conref in another topic. While DITA and Oxygen make no issue of this \(in fact, re-use is recommended\), nested conrefs can become an issue if you open your topics in other programs. Adobe FrameMaker, for instance, is unable to read the nested conref and simply leaves the space blank, leading to incomplete sentences.

**Note:** The same may occur when you cross reference a title containing a conref.

**Parent topic:**[Guidelines for writing in Oxygen XML](../en/to_guidelines_and_tips_oxygen_xml.md)

**Related information**  


[What is content reuse?](co_why_reuse_content.md)

[Different levels of content re-use](co_levels_content_reuse.md)

[The risk: creating conref spaghetti](co_conref_spaghetti.md)

[The solution: a conref library](co_conref_library.md)

[To create a conref library](ta_create_conref_library.md)

