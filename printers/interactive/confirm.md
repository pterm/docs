# Confirm

{% embed url="https://raw.githubusercontent.com/pterm/pterm/master/_examples/interactive_confirm/demo/animation.svg" %}

## Basic Usage

```go
result, _ := pterm.DefaultInteractiveConfirm.Show("Are you sure?")
pterm.Println(result)
```

## Options

| Name              | Type        | Description                                          |
| ----------------- | ----------- | ---------------------------------------------------- |
| `DefaultValue` | `bool` |   |
| `DefaultText`  | `string` |   |
| `TextStyle`    | `*Style` |   |
| `ConfirmText`  | `string` |   |
| `ConfirmStyle` | `*Style` |   |
| `RejectText`   | `string` |   |
| `RejectStyle`  | `*Style` |   |
| `SuffixStyle`  | `*Style` |   |

### Using Options

{% content-ref url="../../tutorials/using-printer-options.md" %}
[using-printer-options.md](../../tutorials/using-printer-options.md)
{% endcontent-ref %}

## Methods

| Method           | Description                                  |
| ---------------- | -------------------------------------------- |
| `Show(text)`        | Displays the interactive confirm prompt                    |

## Full Specification

{% hint style="info" %}
pkg.go.dev contains the full specification for this printer and more technical descriptions.
{% endhint %}

{% embed url="https://pkg.go.dev/github.com/pterm/pterm#InteractiveConfirmPrinter" %}