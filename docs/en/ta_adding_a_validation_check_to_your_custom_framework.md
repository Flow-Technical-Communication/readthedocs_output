---
author: [Pieterjan Vandenweghe, Pieterjan Vandenweghe]
category: DITA
keyword: [Oxygen XML, Schematron, Schematron QuickFix]
---

# To add a validation check to your custom framework

1.  In Oxygen XML, choose **Options** \> **Preferences**.

2.  Go to **Document Type Association**.

3.  Select your document type and click **Edit**.

    DITA for Flow

4.  In the **Validation** tab, click ![](../_media/graphics/oxy_icon_new.png).

5.  Give a name to your new scenario in the **Name** text field, for example Schematron.

6.  Double-click in the first row of the **Schema** column.

7.  Choose **Use custom schema**.

8.  Add the correct Schematron file in the **URL** text field using one of the following options:

    -   Enter the URL in the text field.
    -   Use the **Browse** drop-down button to browse for a local file.
    -   Use the **Insert Editor Variable** button to insert the local file with a editor variable.
9.  Click **OK** \> **OK** \> **OK** \> **Apply** \> **OK**.




**Note:** All Schematron files are saved in the .../\_custom\_framework/dita\_extension/Schematron folder.

**Parent topic:**[Detecting and fixing style guide errors in Oxygen XML](../en/co_validation_checks_in_oxygenxml.md)

