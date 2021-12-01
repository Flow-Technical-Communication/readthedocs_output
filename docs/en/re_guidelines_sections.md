---
author: [Pieterjan Vandenweghe, Pieterjan Vandenweghe]
category: [DITA, DITA]
audience: 
---

# Guidelines for using sections

Concept topics and reference topics can be divided into sections. If you write a reference topic with guidelines for using sections, for example, you can create a separate section for each of these guidelines.

## Add an accurate title

Although it is not mandatory to add a title to a section in DITA, it is recommended. If you use sections in a topic, this normally means that you are dealing with a larger topic. Adding a title to each section then clarifies the structure of the topic and increases its scannability.

For example, you are writing a topic with guidelines for file naming and you created a separate section for each guideline. If you add an accurate title to each section, the reader can use these titles to get an overview of all guidelines.

## Mind Miller's law \(7 ± 2\)

You do not only have to mind Miller's law \(an average person can only hold 7 ± 2 objects in his working memory\) when chunking content, it is also a helpful guideline for creating sections. If your topic has too many sections, you have to organize your content differently. You can, for example split the topic into two smaller topics. Each of these topics will then include fewer sections.

## Evaluate the length

When you have written a multi-section topic, check how long each of your sections is. If the sections are too long or too short, you have to organize your information differently:

|If the sections are...|Do the following...|
|----------------------|-------------------|
|Too long \(several paragraphs, tables, illustrations...\)|Promote each section to a separate topic and group the topics under a parent topic.|
|Too short \(only a few sentences\)|Present the information as a bulleted list or in a table.|

## Do not mind the output

If you generate HTML output from DITA topics, you will normally get a separate HTML page per topic. If you want particular topics to be presented on the same page, you could then make them into sections of a large topic.

This, however, is improper use of DITA: you should never alter the structure of your topics in function of how they will look in the output. You can sort the same effect by setting the `@chunk` attribute to `<to-content>`. The HTML output will then look the way you want it to and your content will still be structured properly.

**Parent topic:**[Guidelines for writing in Oxygen XML](../en/to_guidelines_and_tips_oxygen_xml.md)

