---
author: [Pieterjan Vandenweghe, Pieterjan Vandenweghe]
category: [DITA, DITA]
audience: 
---

# Guidelines for conditional processing

## Define values clearly

When you plan your conditional processing scheme, make sure you have defined all the values before starting the actual writing process. This will make it clear between different writers which attributes should be applied in which situations. If the values are not clearly defined, each writer might start making his own conditional attribute for the same type of content. This situation where separate sets of attributes need to be maintained is called 'condition sprawl' and leads to an unnecessary complication of the attribute system.

**Important:** When defining your values, keep in mind that they are case-sensitive. Therefore 'windows' and 'Windows' will be seen as two separate values. This means that certain information might not get flagged or filtered out correctly.

Without a conditional processing scheme, your writers each make up a different value to apply to Windows-only content of your documentation: 'windows', 'win\_only' and 'win'. You can choose to maintain all three of these values and adjust your DITAVAL accordingly, or you can find all values and change them to one unique value.

## Make efficient use of otherprops

The `@otherprops` attribute can be used to store any other metadata information that does not fit into the standard conditional attributes \(audience, platform, and product\). To extend the functionality of the `@otherprops` attribute, a naming convention can be used that a processor can interpret.

For example, in order to broaden your attribute options, you define the following values for the `@otherprops` attribute: 'Market\(Australia\)' and 'Publication\(Symmetry\). This allows you to use the same attribute for a number of functions. Your processor can now differentiate between "Market" and "Publication".

## Correctly apply conditional attributes in topics

Avoid applying conditions to phrase level elements such as `ph`, `uicontrol`, `filepath` and `userinput`, as filtering out this kind of information can create nonsensical sentences. Instead, apply the condition to the entire sentence and add a similar sentence with a different condition for a different audience, platform etc.

**Tip:** Assign conditional values to your attributes as you write each topic, rather than after you've written dozens or more. Assigning them as you write is faster than trying to hunt down topics that still need conditional attributes at the end.

## Conditional processing versus content referencing

Choose wisely between conditional processing and context referencing. Sometimes it can be easier to adjust one central conref than to create and maintain a system of conditional processing attributes. Each method has its own advantages:

|Conditional processing|Context reference|
|----------------------|-----------------|
|All variations are immediately visible to the author.|Topics are easier for an author to read.|
|A review version of the document can be produced that shows all variations at once.|Does not rely on metadata.|
|Perfectly suited for limited content changes, for instance, alternative installation steps per model.|Can cope better with large numbers of conditions.|
| |Easier to maintain if new variations are introduced as only the conref source file needs to be updated.|

## Correctly apply conditional attributes in DITA maps

If you want to create different output for your DITA map, the easiest method is to make a new DITA map with a different topic structure. Re-using \(and consequently also not re-using\) some topics is easier to maintain than setting up and maintaining a system of conditional processing attributes. In some cases, however, it is more practical to use conditional processing at the level of DITA maps.

In DITA maps, you can apply the conditional attributes to the `topicref` elements in both the hierarchy and in the relationship table. This way you can exclude topics or links from your output.

**Note:** Conditions on the highest level within a DITA map can cause problems when generating your book in Adobe FrameMaker \(FM\). FM reads the condition on a topic and will want to exclude it, but it still reads the topic as being present in its book structure. FM will try to solve this inconsistency by replacing the topic with an empty file containing only a title. You can then just delete this file.

## Don't over-use content flagging

Avoid over-using the option of flagging content: flags are meant to quickly guide a person to the correct information, but too many flags can be distracting and can force the reader to read through a lot of unnecessary information. If you have many flagged items in one topic consider creating different topics, for instance, when you are writing how to install a particular application on several operating systems. Rather than flagging the separate methods for each OS, instead consider writing a new topic for each OS and filtering them with attributes.

To help you decide between flagging or creating separate topics, consider these guidelines:

|If|Then|
|--|----|
|You only have two or three differences in a nine-step task topic|Create one topic and use flagging to highlight the differences.|
|You have more than four differences in a nine-step task topic|Create one topic for each operating system.|

**Parent topic:**[Guidelines for writing in Oxygen XML](../en/to_guidelines_and_tips_oxygen_xml.md)

