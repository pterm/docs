---
description: The table printer can be used to display structured data
---

# Table

{% embed url="https://raw.githubusercontent.com/pterm/pterm/master/_examples/table/demo/animation.svg" %}

## Basic Usage

```go
pterm.DefaultTable.WithData(pterm.TableData{
    {"Paul", "Dean", "nisi.dictum.augue@velitAliquam.co.uk"},
    {"Callie", "Mckay", "egestas.nunc.sed@est.com"},
    {"Libby", "Camacho", "aliquet.lobortis@semper.com"},
}).Render()
```

## Options

| Name              | Type        | Description                                          |
| ----------------- | ----------- | ---------------------------------------------------- |
|	`Style`                  | `*Style` |   |
|	`HasHeader`              | `bool` |   |
|	`HeaderStyle`            | `*Style` |   |
|	`HeaderRowSeparator`     | `string` |   |
|	`HeaderRowSeparatorStyle`| `*Style` |   |
|	`Separator`              | `string` |   |
|	`SeparatorStyle`         | `*Style` |   |
|	`RowSeparator`           | `string` |   |
|	`RowSeparatorStyle`      | `*Style` |   |
|	`Data`                   | `TableData` |   |
|	`Boxed`                  | `bool` |   |
|	`LeftAlignment`          | `bool` |   |
|	`RightAlignment`         | `bool` |   |
|	`Writer`                 | `io.Writer` |   |

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
