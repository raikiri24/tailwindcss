#### Typography

- [Font Weight](#font-weight)
- [Font Style Hover, focus and other states](#font-weight-hover-focus-states)

<h3 style="text-align:center" id="font-weight">Font Weight</h3>
Utilities for controlling the font weight of an element.

| Class              | Properties                                |
| ------------------ | ----------------------------------------- |
| normal-nums        | font-variant-numeric: normal;             |
| ordinal            | font -variant-numeric: ordinal;           |
| slashed-zero       | font-variant-numeric: slashed-zero;       |
| lining-nums        | font-variant-numeric: lining-nums;        |
| oldstyle-nums      | font-variant-numeric: oldstyle-nums;      |
| proportional-nums  | font-variant-numeric: proportional-nums;  |
| tabular-nums       | font-variant-numeric: tabular-nums;       |
| diagonal-fractions | font-variant-numeric: diagonal-fractions; |
| stacked-fractions  | font-variant-numeric: stacked-fractions;  |

Basic usage
​
Applying numeric variants

Use the `font-variant-numeric` utilities to enable additional glyphs for numbers, fractions, and ordinal markers (in fonts that support them).

These utilities are composable so you can enable multiple `font-variant-numeric` features by combining multiple classes in your HTML:

```bash


```

Applying conditionally
​

<h3 style="text-align:center" id="font-weight-hover-focus-states"> Hover, focus, and other states </h3>

Tailwind lets you conditionally apply utility classes in different states using variant modifiers. For example, use `hover:tabular-nums` to only apply the `tabular-nums` utility on hover.

```bash



```

For a complete list of all available state modifiers, check out the [Hover, Focus, & Other States documentation](https://tailwindcss.com/docs/hover-focus-and-other-states).
