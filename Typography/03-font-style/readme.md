#### Typography

- [Font Style](#font-style)
- [Font Style Hover, focus and other states](#font-style-hover-focus-states)

<h3 style="text-align:center" id="font-style">Font Style</h3>
Utilities for controlling the style of text.

| Class      | Properties         |
| ---------- | ------------------ |
| italic     | font-style:italic; |
| not-italic | font-style:normal; |

#### Italicizing text

The `italic` utility can be used to make text italic. Likewise, the `not-italic` utility can be used to display text normally — typically to reset italic text at different breakpoints.

```bash

    <p class="italic">
      Lorem ipsum, dolor sit amet consectetur adipisicing elit. Sapiente illum
      itaque praesentium molestiae! Illum earum modi, id commodi magni sed
      eveniet quaerat aliquam labore ab molestias inventore possimus ea
      provident.
    </p>
    <p class="not-italic">
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Cumque
      perferendis officia odio unde doloremque suscipit consequuntur, sequi
      delectus eveniet aliquid ipsam, vitae eius incidunt voluptate deleniti
      quidem quo aut tempora.
    </p>

```

> CHECK `Typography/font-smoothing.html` to see the result.
> Always run this command in your terminal before checking your page.

```bash
    npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch
```

Applying conditionally

<h3 id="font-style-hover-focus-states"> Hover, focus, and other states</h3>

Tailwind lets you conditionally apply utility classes in different states using variant modifiers. For example, use `hover:not-italic` to only apply the `not-italic` utility on hover.

```bash

  <h1 class="mt-7 font-bold text-3xl">
    FONT STYLE HOVER,FOCUS and OTHER STATE
  </h1>
  <p class="italic hover:not-italic mt-7">HOVER ME!</p>
  <input
    class="not-italic hover:italic mt-7 border-4 border-black"
    placeholder="Click me!"
  />
```

For a complete list of all available state modifiers, check out the [Hover, Focus, & Other States documentation](https://tailwindcss.com/docs/hover-focus-and-other-states).
