---
description: The center printer can be used to center text in the terminal
---

# Center

{% embed url="https://raw.githubusercontent.com/pterm/pterm/master/_examples/center/demo/animation.svg" %}

## Basic Usage

```go
pterm.DefaultCenter.Println("Hello, World!")
```

## Options

| Name                       | Type        | Description                                                           |
| -------------------------- | ----------- | --------------------------------------------------------------------- |
| `CenterEachLineSeparately` | `bool`      | Sets if the printer should center each line separately, or as a block |
| `Writer`                   | `io.Writer` | Sets a custom writer                                                  |

### Using Options

{% content-ref url="../../tutorials/using-printer-options.md" %}
[using-printer-options.md](../../tutorials/using-printer-options.md)
{% endcontent-ref %}

## Methods

{% hint style="info" %}
This printer implements the `TextPrinter` interface.
{% endhint %}

{% content-ref url="./" %}
[.](./)
{% endcontent-ref %}

| Method                                       | Description                                                                                  |
| -------------------------------------------- | -------------------------------------------------------------------------------------------- |
| `Sprint(a ...interface{})`                   | Returns a string                                                                             |
| `Sprintln(a ...interface{})`                 | Returns a string with a new line at the end                                                  |
| `Sprintf(format string, a ...interface{})`   | Returns a string, formatted according to a format specifier                                  |
| `Sprintfln(format string, a ...interface{})` | Returns a string, formatted according to a format specifier with a new line at the end       |
| `Print(a ...interface{})`                    | Prints to the terminal                                                                       |
| `Println(a ...interface{})`                  | Prints to the terminal with a new line at the end                                            |
| `Printf(format string, a ...interface{})`    | Prints to the terminal, formatted according to a format specifier                            |
| `Printfln(format string, a ...interface{})`  | Prints to the terminal, formatted according to a format specifier with a new line at the end |
