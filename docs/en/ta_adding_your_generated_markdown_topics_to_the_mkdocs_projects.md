---
author: [Pieterjan Vandenweghe, Pieterjan Vandenweghe]
keyword: 
---

# Creating the necessary files for the MkDocs projects

You can publish directly in the MkDocs project, but it is not recommended for now because of some minor bugs in the DITA-OT plug-in.

1.  Publish the DITA file with your ReadtheDocs transformation scenario.

2.  Copy the folder with the media objects and the Markdown file into your MkDocs root folder.

    **Note:** Do not copy the YAML file.

3.  Open the YAML file from your DITA publication and copy all files from `pages:`

    **Note:** Do not copy the `theme:` line at the end of the file.

4.  Open the YAML file from your MkDocs project and paste file you copied in step [3](#step_nts_x55_msb).


