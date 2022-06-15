---
description: >-
  The progress bar printer can be used to display the current progress of an
  action
---

# Progressbar

{% embed url="https://raw.githubusercontent.com/pterm/pterm/master/_examples/progressbar/demo/animation.svg" %}

## Basic Usage

```go
progressbar := pterm.DefaultProgressbar.WithTotal(totalSteps).Start()
// Logic here
progressbar.Increment()
// More logic
```

## Options

| Name                        | Type            | Description |
| --------------------------- | --------------- | ----------- |
| `Title`                     | `string`        |             |
| `Total`                     | `int`           |             |
| `Current`                   | `int`           |             |
| `BarCharacter`              | `string`        |             |
| `LastCharacter`             | `string`        |             |
| `ElapsedTimeRoundingFactor` | `time.Duration` |             |
| `BarFiller`                 | `string`        |             |
| `MaxWidth`                  | `int`           |             |
| `ShowElapsedTime`           | `bool`          |             |
| `ShowCount`                 | `bool`          |             |
| `ShowTitle`                 | `bool`          |             |
| `ShowPercentage`            | `bool`          |             |
| `RemoveWhenDone`            | `bool`          |             |
| `TitleStyle`                | `*Style`        |             |
| `BarStyle`                  | `*Style`        |             |
| `IsActive`                  | `bool`          |             |

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

## Full Specification

{% hint style="info" %}
pkg.go.dev contains the full specification for this printer and more technical descriptions.
{% endhint %}

{% embed url="https://pkg.go.dev/github.com/pterm/pterm#ProgressbarPrinter" %}