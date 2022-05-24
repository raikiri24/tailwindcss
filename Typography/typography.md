#### Typography

### Font Family

Utilities for controlling the font family of an element

| Class      | Properties                                                                                                                                                                                                                    |
| ---------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| font-sans  | font-family: ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, "Noto Sans", sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"; |
| font-serif | font-family: ui-serif, Georgia, Cambria, "Times New Roman", Times, serif;                                                                                                                                                     |
| font-mono  | font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace;                                                                                                              |

#### Basic usage

### Setting the font family

You can control the typeface of text using the font family utilities

```bash
   <p class="font-sans">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. (FONT-SANS)
    </p>
    <p class="font-serif">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. (FONT-SERIF)
    </p>
    <p class="font-mono">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. (FONT-MONO)
    </p>
```

> CHECK `Typography/font-family.html` to see the result.
> Always run this command in your terminal before checking your page.

```bash
    npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch
```

Applyying conditionally

#### Hover, focus, and other states

Tailwind lets you conditionally apply utility classes in different states using variant modifiers. For example, use hover:font-serif to only apply the font-serif utility on hover.

```bash
   <p class="font-sans hover:font-mono">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. (FONT-SANS)
    </p>
```

> CHECK `Typography/hover-focus-state.html` to see the result.
> Always run this command in your terminal before checking your page.

```bash
    npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch
```

For a complete list of all available state modifiers, check out the [Hover, Focus, & Other States documentation](https://tailwindcss.com/docs/hover-focus-and-other-states).

Breakpoints and media queries
You can also use variant modifiers to target media queries like responsive breakpoints, dark mode, prefers-reduced-motion, and more. For example, use md:font-serif to apply the font-serif utility at only medium screen sizes and above.

```bash
<p class="font-sans md:font-serif">

  <!-- ... -->
</p>
```

To learn more, check out the documentation on [Responsive Design](https://tailwindcss.com/docs/responsive-design), [Dark Mode](https://tailwindcss.com/docs/dark-mode) and [other media query modifiers](https://tailwindcss.com/docs/hover-focus-and-other-states#media-queries).
