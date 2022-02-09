---
author: [Pieterjan Vandenweghe, Pieterjan Vandenweghe]
keyword: 
---

# Creating a ReadtheDocs transformation scenario in OxygenXML

1.  Open the **Configure Transformation scenario\(s\)** window and select **New** \> **DITA-OT Transformation**.

2.  Select **Markdown for ReadtheDocs**.

3.  Give your new transformation scenario a proper name.

    There are two specific parameter for this ReadtheDocs transformation. When the parameters are empty, the plug-in works with the default ReadtheDocs template and theme. This is fine publication purposes.

    |Parameter|Description|
    |---------|-----------|
    |args.readthedocs.template|Add a link to a configuration YAML file|
    |args.readthedocs.theme|Add the name of a ReadtheDocs theme|

4.  Set the correct **Temporary files directory** and **output** directory in the **Output** tab.

5.  In the **Parameters** tab, select result.rewrite-rule.xsl:

    1.  Add a link an XSLT file with the following code:

        ```xslt
        
        <xsl:stylesheet xmlns:xsl="http://www.w3.org/1999/XSL/Transform"
        	version="2.0">
        <xsl:template match="node() | @*">
        <xsl:copy>
        <xsl:apply-templates select="node() | @*"/>
        </xsl:copy>
        </xsl:template>
        	
        <xsl:template match="file[@format = 'image']/@result">
        <xsl:attribute name="{local-name()}" select="concat('../graphics/',tokenize(../@result, '/')[last()])"/>
        </xsl:template>
        </xsl:stylesheet>
        ```

        You can also link to the existing rewrite-images-readthedocs.xsl file in the com.flow.rewrite.images plug-in the .

6.  In the **Parameters** tab, select **New** and add the following parameters:

    |Parameter|value|
    |---------|-----|
    |dita.flow.rewrite.media|true|
    |dita.flow.rewrite.media.folder|link to a media subfolder of your output folder. The name of the media subfolder should be identical to the folder defined in the XSLT file from step [5](#step_jnt_km5_msb). Based on the current example, this media subfolder is graphics.|

    **Note:** Above parameters only work when the `com.flow.rewrite.images` plugin is installed in your DITA OT.

    This is an example how you have to combine the output directory with thedita.flow.rewrite.media.folder paremeter:

    -   output: \_output/readthedocs/
    -   dita.flow.rewrite.media.folder: \_output/readthedocs/graphics
7.  
