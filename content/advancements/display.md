+++
weight = 2
title = "Display"
prev = "/advancements/introduction"
next = "/advancements"
+++

The `display` object is, as the name implies, pivotal for displaying the advancement in the advancement window, along with any other UI component requiring information about the advancement (such as a toast, another form of notification etc.)

## Example

```json
    "display": {
        "icon": "minecraft:diamond",
        "title": "Diamonds!"
    }
```

## Property List

| Property | Description | Possible Values | Optional? | Example |
| -------- | ----------- | --------------- | :-------: | ------- |
| `icon`   | Specifies the block or item you want the advancement to use as an icon. | Any block or item ID | ✘ | `"icon": "minecraft:diamond"`
| `frame`  | Specifies the type of advancement (along with the frame the icon will use). Also alters the wording of the notification. If this property is omitted, the default frame is `task`. | `task`, `challenge`, `goal` | ✔ | `"frame": "challenge"` |
| `title` | The human-readable title of the advancement | Any string value  | ✘ | `"title": "Diamonds!"` |

## Frame Gallery

| Frame Identifier | Image |
| :--------------: | :---: |
| `task`           | ![Task Frame](../task_frame.png) |
| `challenge`      | ![Challenge Frame](../challenge_frame.png)
| `goal`           | ![Goal Frame](../goal_frame.png)