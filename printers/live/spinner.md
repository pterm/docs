---
description: >-
  The spinner printer can be used to show the user that the program is doing
  something in the background
---

# Spinner

{% embed url="https://raw.githubusercontent.com/pterm/pterm/master/_examples/spinner/demo/animation.svg" %}

## Basic Usage

```go
pterm.DefaultSpinner.Start()
// do something...
pterm.DefaultSpinner.Stop()
```

## Options

| Name                  | Type            | Description |
| --------------------- | --------------- | ----------- |
| `Text`                | `string`        |             |
| `Sequence`            | `[]string`      |             |
| `Style`               | `*Style`        |             |
| `Delay`               | `time.Duration` |             |
| `MessageStyle`        | `*Style`        |             |
| `SuccessPrinter`      | `TextPrinter`   |             |
| `FailPrinter`         | `TextPrinter`   |             |
| `WarningPrinter`      | `TextPrinter`   |             |
| `RemoveWhenDone`      | `bool`          |             |
| `ShowTimer`           | `bool`          |             |
| `TimerRoundingFactor` | `time.Duration` |             |
| `TimerStyle`          | `*Style`        |             |
| `IsActive`            | `bool`          |             |

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
