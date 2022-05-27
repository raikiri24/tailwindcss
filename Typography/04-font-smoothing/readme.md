#### Typography

- [Font Smoothing](#font-smoothing)
- [Font Smoothing Hover, focus, and other states](#font-smoothing-hover-focus-states)

<h3 id="font-smoothing">Font Smoothing</h3>
Utilities for controlling the font smoothing of an element.

| Class                | Properties                                                              |
| -------------------- | ----------------------------------------------------------------------- |
| antialiased          | -webkit-font-smoothing: antialiased;-moz-osx-font-smoothing: grayscale; |
| subpixel-antialiased | -webkit-font-smoothing: auto; -moz-osx-font-smoothing: auto;            |

#### Applying font smoothing

Use the `subpixel-antialiased` utility to render text using subpixel antialiasing and the `antialiased` utility to render text using grayscale antialiasing.

```bash
    <p class="subpixel-antialiased">
      Lorem ipsum dolor sit, amet consectetur adipisicing elit. Consequatur
      sint, deleniti illum tempore dolore ad fugiat ipsa similique atque
      quibusdam doloremque rerum at molestias architecto ut sed. Eum, dicta
      pariatur?
    </p>
    <p class="antialiased">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Qui cum
      reiciendis doloribus earum unde voluptatibus dolore fuga amet minima
      tempore eveniet temporibus quidem incidunt quo dignissimos eligendi,
      aperiam minus eos.
    </p>
```

> CHECK `Typography/font-smoothing.html` to see the result.
> Always run this command in your terminal before checking your page.

```bash
    npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch
```

Applying conditionally

<h3 id="font-smoothing-hover-focus-states"> Hover, focus, and other states</h3>

Tailwind lets you conditionally apply utility classes in different states using variant modifiers. For example, use `hover:subpixel-antialiased` to only apply the `subpixel-antialiased` utility on hover.

```bash

    <p class="antialiased hover:subpixel-antialiased mt-7">HOVER ME!</p>

    <input
      class="subpixel-antialiased hover:antialiased mt-7 border-4 border-black"
      placeholder="Click me!"
    />
```

For a complete list of all available state modifiers, check out the [Hover, Focus, & Other States documentation](https://tailwindcss.com/docs/hover-focus-and-other-states).
