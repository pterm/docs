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

| Name              | Type        | Description                                          |
| ----------------- | ----------- | ---------------------------------------------------- |
| `TextStyle`       | `*Style`    | Style of the text                                    |
| `BackgroundStyle` | `*Style`    | Style of the header background                       |
| `Margin`          | `int`       | Empty space to the sides                             |
| `FullWidth`       | `bool`      | Sets if the header should be as wide as the terminal |
| `Writer`          | `io.Writer` | Sets a custom writer                                 |

### Using Options

{% content-ref url="../../tutorials/using-printer-options.md" %}
[using-printer-options.md](../../tutorials/using-printer-options.md)
{% endcontent-ref %}

## Methods

{% hint style="info" %}
This printer implements the `RenderablePrinter` interface.
{% endhint %}

| Method      | Description                                           |
| ----------- | ----------------------------------------------------- |
| `Render()`  | Prints to the terminal or uses the specified `Writer` |
| `Srender()` | Returns the rendered string                           |
