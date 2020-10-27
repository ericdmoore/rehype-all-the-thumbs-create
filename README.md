# rehype-all-the-thumbs-create
Supporting [`rehype-all-the-thumbs`](https://github.com/ericdmoore/rehype-all-the-thumbs) by creating the thumbnails based on the input elements

> rehype-👍🏿👍🏼👍🏽👍🏻👍🏾 (make new vfiles based on inputs)

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

## Pairs Well With:

- [rehype-all-the-thumbs](https://github.com/ericdmoore/rehype-all-the-thumbs) ...like putting on velcro shoes
- [rehype-all-the-thumbs-curate](https://github.com/ericdmoore/rehype-all-the-thumbs-curate) (DOM -> data.srcs)
- [rehype-all-the-thumbs-manipulate](https://github.com/ericdmoore/rehype-all-the-thumbs-manipulate) (data.newAssets -> DOM)
- [rehype-all-the-thumbs-obviate](https://github.com/ericdmoore/rehype-all-the-thumbs-obviate) (data.newAssets.filter -> data.newAssets)
- [vfile-newAssets-generate](https://github.com/ericdmoore/vfile-newAssets-generate) (data.newAssets -> Side Effect Funtion to create the file)
