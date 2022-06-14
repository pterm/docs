---
description: The prefix printer can be used to display prefixed messages
---

# Prefix

{% embed url="https://raw.githubusercontent.com/pterm/pterm/master/_examples/prefix/demo/animation.svg" %}

## Basic Usage

```go
pterm.Debug.Println("Hello, World!") // Print Debug.
pterm.Info.Println("Hello, World!") // Print Info.
pterm.Success.Println("Hello, World!") // Print Success.
pterm.Warning.Println("Hello, World!") // Print Warning.
pterm.Error.Println("Hello, World!") // Print Error.
pterm.Fatal.Println("Hello, World!") // Print Fatal.                                             // Print Fatal.
```

## Options

| Name               | Type        | Description                                                                             |
| ------------------ | ----------- | --------------------------------------------------------------------------------------- |
| `Prefix`           | `Prefix`    | The styled prefix that should be used in front of messages                              |
| `Scope`            | `Scope`     | The optional scope that should be used when printing                                    |
| `MessageStyle`     | `*Style`    | The style of the message                                                                |
| `Debugger`         | `bool`      | Sets if the prefix printer should only print when PTerm's debug mode is active          |
| `Fatal`            | `bool`      | Sets if the prefix printer should stop the program                                      |
| `ShowLineNumber`   | `bool`      | Sets if the prefix printer should display the file and line number, where it was called |
| `LineNumberOffset` | `int`       | Sets how many steps in the stack trace should be ignored                                |
| `Writer`           | `io.Writer` | Sets a custom writer                                                                    |

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
