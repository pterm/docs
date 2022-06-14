---
description: The tree printer can be used to display a hierarchy
---

# Tree

{% embed url="https://raw.githubusercontent.com/pterm/pterm/master/_examples/tree/demo/animation.svg" %}

## Basic Usage

```go
pterm.DefaultTree.WithRoot(putils.NewTreeFromLeveledList(pterm.LeveledList{
    pterm.LeveledListItem{Level: 0, Text: "Hello, World!"}
    pterm.LeveledListItem{Level: 1, Text: "Hello, World2!"}
})).Render()
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
