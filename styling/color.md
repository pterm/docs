---
description: This page describes how you can use PTerm to print colored output
---

# Color

## Color Type

{% embed url="https://raw.githubusercontent.com/pterm/pterm/master/_examples/coloring/demo/animation.svg" %}
[https://github.com/pterm/pterm/tree/master/\_examples/coloring/demo](https://github.com/pterm/pterm/tree/master/\_examples/coloring/demo)
{% endembed %}

{% hint style="info" %}
PTerms color type is safe to use on every terminal that supports colored text. It follows the ANSI specifications and  is very simple to use.
{% endhint %}

## RGB Type

{% embed url="https://raw.githubusercontent.com/pterm/pterm/master/_examples/coloring/fade-multiple-colors/animation.svg" %}
[https://github.com/pterm/pterm/tree/master/\_examples/coloring/fade-multiple-colors](https://github.com/pterm/pterm/tree/master/\_examples/coloring/fade-multiple-colors)
{% endembed %}

{% hint style="info" %}
PTerms RGB type supports all 8 million colors of the RGB specification. It is not supported on older terminals, but PTerm will automatically convert it to the nearest ANSI color, if RGB is not supported.
{% endhint %}



## Style Type

{% hint style="info" %}
PTerms style type is a collection of foreground colors, background colors and decorators. It can be used to combine ANSI colors.
{% endhint %}

