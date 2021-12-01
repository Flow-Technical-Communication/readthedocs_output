---
author: Pieterjan Vandenweghe
category: DITA
keyword: [glossentry, glossterm, glossdef, Oxygen XML]
---

# To create a glossary

1.  Create a new ditamap.

    **Note:** You can give this ditamap any name you like, but for clarity’s sake, we suggest you call it \_Glossary.

2.  Create a glossary topic.

    **Note:** You can simply name this topic to\_glossary.dita.

3.  Append the topic to the glossary ditamap.

4.  Create glossentry topics:

    1.  Choose **File** \> **New**.

    2.  Go to **Framework templates** \> **DITA** \> **Topics**.

    3.  Select **Glossentry**.

    4.  Enter a title.

        **Note:** Start your title with gl\_ to easily recognize glossary term files.

    5.  Click **Create**.

        In the **DITA Maps Manager**, Oxygen opens a glossentry file.

    6.  Enter a term in the `glossterm` element.

    7.  Enter a definition in the `glossdef` element.

    8.  Enter extra `glossentry` elements, if necessary.

5.  Append the glossentry topics to the glossary topic.

6.  Define a key for each glossentry topic:

    1.  Right-click the topic and select **Edit properties...**.

    2.  Go to the tab **Keys** and enter a key in the **Define keys:** field.

        **Note:** You can give this `@keys` attribute any name you like, but for clarity’s sake, we suggest you give it the same name as its `glossterm` or title. Start the key with `gl_` to easily find it in the key list.

    3.  Select **OK**.


**Parent topic:**[Adding glossaries through tooltips](../en/to_glossaries_through_tooltips.md)

**Related information**  


[To create a new topic](ta_to_create_new_topic.md)

[To add a topic to a DITA map](ta_to_add_a_topic_to_a_ditamap.md)

[What are glossaries?](co_what_are_glossaries.md)

[To reference a glossary term in a topic](ta_reference_term_in_topic.md)

[To group glossary terms on a single output page](ta_glossary_one_page.md)

[To create a new DITA map](ta_to_create_a_ditamap.md)

[Extra term information](co_additional_term_information.md)

[Variants of a term](co_variant_of_term.md)

