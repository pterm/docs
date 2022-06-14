---
description: >-
  The panel printer can be used to create multiple spaces in the terminal, which
  can have different content
---

# Panel

{% embed url="https://raw.githubusercontent.com/pterm/pterm/master/_examples/panel/demo/animation.svg" %}

## Basic Usage

```go
// Declare panels in a two dimensional grid system.
panels := pterm.Panels{
  {{Data: "This is the first panel"}, {Data: pterm.DefaultHeader.Sprint("Hello, World!")}, {Data: "This\npanel\ncontains\nmultiple\nlines"}},
  {{Data: pterm.Red("This is another\npanel line")}, {Data: "This is the second panel\nwith a new line"}},
}

// Print panels.
pterm.DefaultPanel.WithPanels(panels).Render()
```

## Options

| Name              | Type         | Description |
| ----------------- | ------------ | ----------- |
| `Panels`          | `Panels`     |             |
| `Padding`         | `int`        |             |
| `BottomPadding`   | `int`        |             |
| `SameColumnWidth` | `bool`       |             |
| `BoxPrinter`      | `BoxPrinter` |             |
| `Writer`          | `io.Writer`  |             |

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
