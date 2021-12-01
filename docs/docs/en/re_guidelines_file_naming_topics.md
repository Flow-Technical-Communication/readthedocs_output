---
author: [Pieterjan Vandenweghe, Pieterjan Vandenweghe]
category: [DITA, DITA]
audience: 
---

# Guidelines for file naming

When using DITA, you create a separate file per topic. It is important to name these files consistently, especially when more writers are contributing topics to the same project. When fixing a syntax for your file names, take into account the following guidelines:

-   Use a prefix that identifies the information type of the topic. You can, for example use to\_ for generic topics, ta\_ for task topics, co\_ for concept topics and re\_ for reference topics.
-   Use short and descriptive names. A shortened version of the topic title, for example, is easily recognizable to yourself and to your fellow authors.
-   Only use lower case characters.
-   Use underscores instead of spaces and avoid special \(non-ASCII\) characters.
-   Use the extension .dita \(recommended\) or .xml.
-   Start the names of special topics \(for example conref library\), bookmaps and DITA maps with an exclamation mark. This makes these files appear on top when you sort them by name.

|Topic title|Information type|Filename|
|-----------|----------------|--------|
|About this manual|Generic topic|to\_about\_this\_manual.dita|
|How to insert batteries in your camera|Task topic|ta\_how\_to\_insert\_batteries.dita|
|What is white balance?|Concept topic|co\_white\_balance.dita|
|Overview of battery icons|Reference topic|re\_overiew\_battery\_icons.dita|
|Conref library|Composite topic|!conref\_library.dita|

**Parent topic:**[Guidelines for writing in Oxygen XML](../en/to_guidelines_and_tips_oxygen_xml.md)

