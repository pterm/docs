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

| Name                   | Type        | Description |
| ---------------------- | ----------- | ----------- |
| `Root`                 | `TreeNode`  |             |
| `TreeStyle`            | `*Style`    |             |
| `TextStyle`            | `*Style`    |             |
| `TopRightCornerString` | `string`    |             |
| `TopRightDownString`   | `string`    |             |
| `HorizontalString`     | `string`    |             |
| `VerticalString`       | `string`    |             |
| `RightDownLeftString`  | `string`    |             |
| `Indent`               | `int`       |             |
| `Writer`               | `io.Writer` |             |

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

## Full Specification

{% hint style="info" %}
pkg.go.dev contains the full specification for this printer and more technical descriptions.
{% endhint %}

{% embed url="https://pkg.go.dev/github.com/pterm/pterm#TreePrinter" %}