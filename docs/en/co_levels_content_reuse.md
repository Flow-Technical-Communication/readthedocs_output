---
author: Pieterjan Vandenweghe
category: DITA
audience: 
---

# Different levels of content re-use

## Re-using elements

On the smallest scale, you can reference a single word or phrase. This should be done with care, however, as conreffing these can lead to some problems, as discussed in [Guidelines for using content references](re_guidelines_content_reference.md#). To avoid creating ungrammatical sentences, it is safest to stick to fixed nouns, names and phrases that are unlikely to be modified by grammar, such as:

|Commonly re-used elements|Examples|
|-------------------------|--------|
|`cite`|Titles of books|
|`filepath`|File, directory or path names|
|`keyword`|Product names, model numbers|
|`menucascade` and `uicontrol`|Interface buttons, menus, check boxes, tabs|
|`wintitle`|Names of windows, panels, pages or dialog boxes|

On a larger scale, commonly referenced elements include:

-   Lists
-   Steps
-   Tables
-   Sentences
-   Paragraphs

## Re-using topics

Re-using topics is a very good way of making efficient use of your content. When you write your content according to the best-practice suggestions, your topics will be clear and self-contained, meaning they can easily be re-used elsewhere and still make sense.

The main way you can re-use a topic is by inserting it into multiple DITA maps. This way you essentially have a single repository of topics, and you link the ones you need in the relevant DITA map\(s\).

![](../_media/graphics/reusing_topics.PNG)

There are types of topics that respond very well to being re-used like this, for instance:

-   Topics that contain standard text, such as legal information.
-   Topics with a recurring information set, such as a procedure that must be done in multiple task flows or scenarios.
-   Topics that need to appear in different sets of information. For example, when you need to add the same topic in an installation guide and a user guide.

**Tip:** If you have a similar topic but with content that needs to be customized, you can create a DITA template instead. Writers can re-use that template to make similarly structured topics but with unique content.

**Note:** Using the same topic several times in the same DITA map can create problems when generating output \(all links to the topic will point to the first instance of the topic\). If you need the same topic to appear several times in the same map, you should use the `@copy-to` attribute. You enter a new filename in the copy-to attribute of the `topicref` element. In this way, you create duplicate topic references in the DITA map without actually creating additional topics in the source files. You can then use the `linktext` and `shortdesc` elements in the `topicmeta` element of the topic reference to provide a unique title and short description to help you distinguish between the two in link previews.

## Re-using DITA maps

You can re-use entire DITA maps in your structure. To create re-usable DITA maps, create and organize topics into submaps that document common features or user tasks. For example, even if you have only one user guide, you can create one DITA map for installation topics, one DITA map for security topics, and one DITA map for configuration topics.

## Re-using content from non-DITA sources

You can re-use existing content such as product codes and external sources by automatically pulling it into your DITA topics. For example, instead of writing a programming reference guide from scratch, you might pull comments from the software code and use those comments in your DITA topics.

Because DITA is a semantic tagging language, it can easily map non-DITA content to the proper DITA elements and insert the content in the correct location in your DITA topics.

**Related information**  


[What is content reuse?](co_why_reuse_content.md)

[Guidelines for using content references](re_guidelines_content_reference.md)

[The risk: creating conref spaghetti](co_conref_spaghetti.md)

[The solution: a conref library](co_conref_library.md)

[To create a conref library](ta_create_conref_library.md)

