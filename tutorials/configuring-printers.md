---
description: This page explains how to customize printers with options
---

# Configuring Printers

{% hint style="info" %}
The printers in PTerm can be configured with options. All printers follow a specific scheme.
{% endhint %}

## Option Scheme

To get a new printer, with custom configuration, you can fork the existing `Default` variant of the printer and modify the option via its `WithXxx` methods.

```go
pterm.DefaultXxx.WithXxx(option)
```

If you want to set multiple options, you can chain them:

```go
pterm.DefaultXxx.WithOption(option).WithOption2(option2)
```

## Overwriting Default Options

{% hint style="info" %}
You can overwrite options of the `Default` printers. Those options will be applied globally. This can be used to modify the style or default values.
{% endhint %}

To overwrite an option of a default printer, you can assign a forked printer to the default printer variable.

### Syntax

```go
pterm.DefaultXxx = *pterm.DefaultXxx.WithXxx(option)
```

### Example

```go
pterm.DefaultHeader = *pterm.DefaultHeader.WithBackgroundStyle(pterm.NewStyle(pterm.BgBlue))
```
