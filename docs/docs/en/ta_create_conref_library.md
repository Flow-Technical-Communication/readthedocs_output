---
author: Pieterjan Vandenweghe
category: DITA
audience: 
---

# To create a conref library

To keep track of all your re-used elements, you can create a conref library. A conref library or warehouse is organized by logical group \(steps, notes, images\) or by products \(product A, product B\). Reusable components of each group are saved in a topic dedicated to the group. A typical warehouse file has the following outline:

![](../_media/graphics/warehouse.png)

To create a warehouse, do the following:

1.  Choose **File** \> **New**.

2.  Go to **Framework Templates** \> **DITA** \> **Maps**.

3.  Choose **Map**.

4.  Enter the name "!warehouse.ditamap".

    **Tip:** Adding an exclamation mark to your filename ensures the file appears at the top of your list of files in your folder, making it easier to find.

5.  Choose a folder specific for warehouses to save the library.

6.  Click **Create**.

7.  Right-click the warehouse map in the **DITA Maps Manager** and choose **Append Child** \> **New**.

8.  Go to **Framework Templates** \> **DITA for Flow** \> **topic\_templates**.

9.  Choose 'topic\_flow'.

10. Enter a name and choose the "\_warehouse" folder to save the library.

    **Tip:** Choose a name which represents the groups of reusable components you are going to store in the file, such as "warehouse\_steps".

11. Click **Create**.

12. Click **Edit Properties**.

13. Choose **Key definition** next to Reference type.

14. Go to the Key tab and type in your type of key next to Define keys.

    For example, when creating a step warehouse, the keys you create are "steps".

15. Go to the Attributes tab and enter **Resource-only** for the `@processing-role` attribute.

16. Click **Create**.

17. Repeat step [7](#step_gzh_ry1_q4b)-[16](#step_hmh_wy1_q4b) for each type of warehouse you want to create.

18. Fill the warehouses while you write by immediately adding elements you intend to re-use in other topics to the warehouses.

19. Give each element an ID by right-clicking it and choosing **Generate IDs**.


**Related information**  


[How is the Mo-vis custom framework built?](co_flow_custom_framework.md)

[The solution: a conref library](co_conref_library.md)

