---
description: The bar chart printer can be used to show data in relation to each other
---

# BarChart

{% embed url="https://raw.githubusercontent.com/pterm/pterm/master/_examples/barchart/demo/animation.svg" %}

## Basic Usage

```go
positiveBars := pterm.Bars{
	pterm.Bar{
		Label: "Bar 1",
		Value: 5,
	},
	pterm.Bar{
		Label: "Bar 2",
		Value: 3,
	},
	pterm.Bar{
		Label: "Longer Label",
		Value: 7,
	},
}

pterm.Info.Println("Chart example with positive only values (bars use 100% of chart area)")

pterm.DefaultBarChart.WithBars(positiveBars).Render()
pterm.DefaultBarChart.WithHorizontal().WithBars(positiveBars).Render()
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
