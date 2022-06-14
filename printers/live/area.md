---
description: The area printer can be used to display dynamically updating live content
---

# Area

{% embed url="https://raw.githubusercontent.com/pterm/pterm/master/_examples/area/demo/animation.svg" %}

## Basic Usage

```go
pterm.DefaultBox.Println("Hello, World!")
```

## Options

| Name                      | Type        | Description |
| ------------------------- | ----------- | ----------- |
|	`RemoveWhenDone` | `bool` |   |
|	`Fullscreen`     | `bool` |   |
|	`Center`         | `bool` |   |

### Using Options

{% content-ref url="../../tutorials/using-printer-options.md" %}
[using-printer-options.md](../../tutorials/using-printer-options.md)
{% endcontent-ref %}

## Methods

{% hint style="info" %}
This printer implements the `LivePrinter` interface.
{% endhint %}

{% content-ref url="./" %}
[.](./)
{% endcontent-ref %}

| Method           | Description                                  |
| ---------------- | -------------------------------------------- |
| `Start()`        | Returns itself and errors                    |
| `Stop()`         | Returns itself and errors                    |
| `GenericStart()` | Returns the started `LivePrinter` and errors |
| `GenericStop()`  | Returns the stopped `LivePrinter` and errors |
