# Text Printers

{% hint style="info" %}
Text printers are printers, which can be used like the standard library's `fmt` package. They have functions, such as `Print()`, `Sprint()`, `Println()`, `Sprintln()`, `Printf()`, `Sprintf()`, `Printfln()`, `Sprintfln()`, etc.
{% endhint %}

## Interface

{% hint style="info" %}
PTerm exposes a `TextPrinter` interface.
{% endhint %}



| Function                                     | Description                                                                                  |
| -------------------------------------------- | -------------------------------------------------------------------------------------------- |
| `Sprint(a ...interface{})`                   | Returns a string                                                                             |
| `Sprintln(a ...interface{})`                 | Returns a string with a new line at the end                                                  |
| `Sprintf(format string, a ...interface{})`   | Returns a string, formatted according to a format specifier                                  |
| `Sprintfln(format string, a ...interface{})` | Returns a string, formatted according to a format specifier with a new line at the end       |
| `Print(a ...interface{})`                    | Prints to the terminal                                                                       |
| `Println(a ...interface{})`                  | Prints to the terminal with a new line at the end                                            |
| `Printf(format string, a ...interface{})`    | Prints to the terminal, formatted according to a format specifier                            |
| `Printfln(format string, a ...interface{})`  | Prints to the terminal, formatted according to a format specifier with a new line at the end |
