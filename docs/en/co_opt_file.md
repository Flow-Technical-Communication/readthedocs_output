# What is a template descriptor file?

The template descriptor file defines the metadata associated with the template, as well as the resources included in the template \(CSS files, JS files, images and transformation parameters\):

```
<?xml version="1.0" encoding="UTF-8" standalone="yes"?>
<publishing-template>
  <name>your_project</name>
  <description>your_project webhelp reponsive customization</description>
  <webhelp>
    <preview-image file="image/your_project-logo.png"/>
    <html-page-layout-files>
      <page-layout-file page="search" file="page-templates/wt_search.html"/>
      ...
    </html-page-layout-files>

    <parameters>
      <parameter name="webhelp.show.main.page.tiles" value="yes"/>
      ....
    </parameters>
    <html-fragments>
      <fragment file="webhelp-fragment/webhelp.fragment.footer.xhtml" placeholder="webhelp.fragment.footer"/>
      ...
    </html-fragments>
    <resources>
      <css file="your_project.css"/>
      <fileset>
        <include name="image/**/*"/>
       ...
      </fileset>
    </resources>
    <online-preview-url>https://www.oxygenxml.com/samples/DITA-WebHelp-Responsive/tiles/aquamarine/</online-preview-url>
    <tags>
      <tag type="layout">tiles</tag>
      ...
    </tags>
  </webhelp>
</publishing-template>

```

**Attention:** The template descriptor file must have the .opt extension and must be located in the template's root folder.

The .opt file contains the following elements:

-   `<name>`: name of your project
-   `<description>`: description of your project
-   `<preview-image>`: image displayed in the **templates** tab of the **Edit DITA scenario** window
-   `<html-page-layout-files>`: files defining the layout of the webhelp pages

    **Note:** These files are stored in the **page-templates** folder.

-   `<parameters>`: parameters of the webhelp transformation scenario \(see [To change the parameters of a transformation scenario](ta_change_parameters_webhelp_transformation.md)\)
-   `<html-fragments>`: files defining fragments of the webhelp

    **Note:** These files are stored in the **webhelp-fragment** folder.

-   `<resources>`: resources of the webhelp, including the custom .css file

    **Note:** When renaming the .css file, you have to adjust the code in the .opt file as well.

-   `<online-preview-url>`: url of the online preview
-   `<tags>`: tags used to filter in the **Edit DITA scenario** window

