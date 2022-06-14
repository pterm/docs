---
description: The bullet list printer can be used to display a bullet list
---

# BulletList

{% embed url="https://raw.githubusercontent.com/pterm/pterm/master/_examples/bulletlist/demo/animation.svg" %}

## Basic Usage

```go
pterm.DefaultBulletList.WithItems([]pterm.BulletListItem{
    {Level: 0, Text: "Level 0"},
    {Level: 1, Text: "Level 1"},
    {Level: 2, Text: "Level 2"},
}).Render()
```

## Options

| Name          | Type               | Description |
| ------------- | ------------------ | ----------- |
| `Items`       | `[]BulletListItem` |             |
| `TextStyle`   | `*Style`           |             |
| `Bullet`      | `string`           |             |
| `BulletStyle` | `*Style`           |             |
| `Writer`      | `io.Writer`        |             |

### Using Options

{% content-ref url="../../tutorials/using-printer-options.md" %}
[using-printer-options.md](../../tutorials/using-printer-options.md)
{% endcontent-ref %}

## Methods

{% hint style="info" %}
This printer implements the `RenderablePrinter` interface.
{% endhint %}

{% content-ref url="./" %}
[.](./)
{% endcontent-ref %}

| Method      | Description                                           |
| ----------- | ----------------------------------------------------- |
| `Render()`  | Prints to the terminal or uses the specified `Writer` |
| `Srender()` | Returns the rendered string                           |
