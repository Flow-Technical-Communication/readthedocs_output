---
author: [Pieterjan Vandenweghe, Pieterjan Vandenweghe]
keyword: 
---

# Link to media files is broken

## Condition

The link to your media object is not correct in the generated Markdown files.

## Cause

The DITA-OT plug-in moves all Markdown files in the docs subfolder as the last step of the transformation process, but does not moves the media object along.

## Remedy

1.  Move the folder with the media objects in the docs subfolder.

    The link to media objects work correctly.


