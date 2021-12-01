# To change the parameters of a transformation scenario

You can change the transformation parameters in the template descriptor file \(see [What is a template descriptor file?](co_opt_file.md)\) by simply adding the `<parameters>` element within the `<webhelp>` element:

```
<parameters>
  <parameter name="webhelp.show.main.page.tiles" value="yes"/>
</parameters>
```

This method is preferred, because all scenario's based on this template will be adjusted. However, you can also adjust the transformation parameters while editing the transformation:

1.  Select ![](../_media/graphics/configure_transformation_scenario.PNG).

2.  Select a transformation scenario under **Project**.

3.  Select **Edit**.

4.  Select the **Parameters** tab.

5.  In the first field, enter the name of your custom .css file \(see [What is a CSS file?](co_custom_css_file.md)\).

    **Note:** Click ![](../_media/graphics/browse.png) to browse for you .css file.

6.  In the **Type filter text** field, you can filter for a parameter you want to adjust.

7.  Select the **Value** field for a parameter and select a new value in the **Value** dropdown list.

8.  Select **Ok** in the **Edit parameter** field.

9.  Select **Ok** in the **Edit DITA scenario** field.


For example, the parameter **args.figurelink.style** specifies how cross references to figures are styled in the output. In the dropdownlist, you can choose to display cross references as the title of the figure, the number of the figure or both.

