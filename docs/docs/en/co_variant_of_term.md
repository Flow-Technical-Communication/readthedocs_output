---
keyword: [glossAlt, glossUsage, glossAbbreviation, glossAcronym, glossAlternateFor, glossShortForm, glossSynonym, glossProperty, glossStatus]
---

# Variants of a term

Variants of a term are contained within the `glossAlt` element:

|Element|Description|
|-------|-----------|
|`glossUsage`|Provides info about the correct use of a term.|
|`glossAbbreviation`|Provides an abbreviated form of the term.|
|`glossAcronym`|Provides an acronym of the term.|
|`glossAlternateFor`|Indicates when a variant term also has a relationship to another variant term. You can link this other variant term with the `@href` or `@keyref` attribute.|
|`glossShortForm`|Provides a shorter alternative to the term.|
|`glossSynonym`|Provides a synonym of the term.|
|`glossProperty`|Provides additional details to the term by providing an extension point. Enter a name and value for the property in the **Text** mode, for example: ```
 <glossProperty name="gender" value="masculine"/>
```

|
|`glossStatus`|Identifies the usage status of a term. Enter a value in the **Text** mode, for example: ```
<glossStatus value="prohibited"/>
```

|

**Related information**  


[General glossary elements](co_including_glossary.md)

[Extra term information](co_additional_term_information.md)

[To create a glossary](ta_creating_a_glossary.md)

