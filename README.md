# rehype-all-the-thumbs-create
Supporting `rehype-all-the-thumbs` by creating the thumbnails based on the input elements

## Overview

_Configuration_:
- a default `srcs` set

_Input_:
- a HAST tree
- vfile with `srcs` instructions

_Output_:
- unchanged HAST tree
- vfile with added `newAssets` key added to the object

## newAssets

- `newAssets` is a `vfile[]` 
- Each `vfile` follows the instructions in the srcs array. Making the right file based on image format, name, etc.
