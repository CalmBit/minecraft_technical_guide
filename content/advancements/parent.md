+++
weight = 4
title = "Parent"
prev = "/advancements/display"
next = "/advancements/criteria"
+++

The `parent` property is a string, listing the name of the advancement this advancement extends from (i.e. the literal "parent" of the advancement in the [tree](/advancements/terminology/#advancement_tree)).

{{% notice note %}}
Technically this *is* an optional property, but any advancement *without* this property will be interepreted as a [root advancement](/advancements/terminology/#root_advancement), which consequently require the absence of this property to be recognized.
{{% /notice %}}

## Example

```json
    "parent": "minecraft:story/iron_tools"
```