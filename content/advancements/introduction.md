+++
weight = 1
title = "Introduction"
prev = "/advancements"
next = "/advancements/terminology"
+++


The Advancements system is a recently added feature that supersedes the previous Achievements system, giving mapmakers (and modders) more flexibility within the Vanilla framework. Advancements can serve an assortment of purposes, including:

* quest-lines
* keeping track of progressions
* introducing fun challenges into vanilla survival

The files are a little complex, but we'll discuss each component in depth, and make it a little less scary.

## The Format

Advancements, being so extremely flexible, utilize [JSON](http://www.json.org/) as an encoding format. They're designed for a great deal of modularity, allowing for as few (or as many) options as necessary. A rudimentary advancement file looks like this:

```json
{
    "display": {
        "icon": "minecraft:diamond",
        "title": "Diamonds!"
    },
    "parent": "minecraft:story/iron_tools",
    "criteria": {
        "diamond": {
            "trigger": "minecraft:inventory_changed",
            "conditions": {
                "items": [
                    {
                        "item": "minecraft:diamond"
                    }
                ]
            }
        }
    }
}
```

This particular advancement supersedes the "DIAMONDS!" achievement, working exactly the same.