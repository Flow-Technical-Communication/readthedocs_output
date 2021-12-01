---
author: [Pieterjan Vandenweghe, Pieterjan.vandenwegh]
keyword: [Standardization, Oxygen XML]
---

# How is the Mo-vis custom framework built?

## About the custom framework

The custom framework is a predefined structure to write multilingual DITA documentation in a efficient way.

The custom framework is on top of that a handy customization of an Oxygen XML framework with predefined settings, such as:

-   Topic templates
-   Oxygen XML webhelp responsive template
-   MiramoPDF template
-   Transformation scenarios with standardized output folders
-   Schematron checks
-   Toolbar

**Note:** The root folder contains two more files:

-   .gitignore: specifies intentionally untracked files that Git should ignore
-   README.md: a markdown file containing general information

## Oxygen XML project file \(\*.xpr\)

In the root folder you find the Oxygen XML project file: movis.xpr . Using this file has a lot of advantages, such as:

-   You can store all project related information, for example settings, code templates and transformation scenarios.
-   You can run batch validations and batch publications.
-   You can run a search and replace on project level.
-   You can define master files which will be updated and relinked when you rename topics or move topics to another folder.
-   When you open the XPR file in Oxygen XML, it will also open all the files that you had open in the project the previous time you used it.

**Tip:** Make sure this project file is opened at any time in Oxygen XML.

## Advantages of a custom framework

Using the custom framework has the following advantages:

-   The custom framework is a kind of a template. You can start your project immediately with all settings and structures set correctly from the start.
-   You can easily collaborate with colleagues in the same project without having to doubt if anyone is following the correct rules.
-   You can easily take over a project from colleagues if they are absent for a while since everyone is using the same basic structure.

