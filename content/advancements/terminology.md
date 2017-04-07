+++
weight = 2
title = "Terminology"
prev = "/advancements/introduction"
next = "/advancements/display"
+++

In order to dicuss advancements in detail, some basic terms will need to be defined - this section is for that exactly. Suspect terms (those with complex or otherwise incomprehensible meaning) will be defined here, and will always contain links to their respective entries.

## <a id="advancement_tree"></a>Advancement Tree

An **advancement tree** is a set of advancements that are descended or ascended from each other, extending from a singular [root advancement](#root_advancement).

## <a id="fully_qualified_path"></a>Fully Qualified Path

An advancement's **fully qualified path** is the full text of the advancement's resource location, including its namespace and sub-folders (e.g. `namespace:folder_one/folder_two/advancement`). These paths are used as definitive, unique locators for several purposes, including defining an advancement's [parent](/advancements/parent).

## <a id="namespace"></a>Namespace

A **namespace** is the overarching label for a group of advancements. For player-made advancements, the namespace is the name of the folder holding the JSON files for the advancements. Official advancements have the namespace `minecraft` (e.g. `minecraft:diamonds`). 

A namespace can be sub-divided into folders (in any number of ways), but these *do not* affect the namespace title, but rather the [fully qualified path](#fully_qualified_path) of the advancement.

{{% notice warning %}}
It's not advised to infringe on the official namespace - this hasn't been tested, but chances are it will cause far more confusion than it's worth.
{{% /notice %}}

## <a id="root_advancement"></a>Root Advancement

The **root advancement** is the first advancement in a particular [advancement tree](#advancement_tree). When its criteria are fufilled, a new tab is added to the advancement window, bearing both its `name` and its `icon` properties. A [namespace](#namespace) can have more than one root advancement, but this could be undesirable for a number of reasons.

## <a id="toast"></a>Toast
A **toast** is defined as a "non modal, unobtrusive window element used to display brief, auto-expiring windows of information to a user." For the purposes of the advancements system, a toast looks like this:

![An example of a toast](/advancements/toast.png)