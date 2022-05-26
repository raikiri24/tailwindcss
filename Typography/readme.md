#### Typography

- [Font Family](#font-family)
- [Font Family Hover, focus, and other states](#font-family-hover-focus-states)
- [Font Size](#font-size)
- [Font Size Hover, focus, and other states](#font-size-hover-focus)
- [Font Smoothing](#font-smoothing)
- [Font Smoothing Hover, focus, and other states](#font-smoothing-hover-focus-states)
- [Font Style](#font-style)
- [Font Style Hover, focus and other states](#font-style-hover-focus-states)

<h3 id="font-family">Font Family</h3>

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

Applying conditionally

<h3 id="font-family-hover-focus-states"> Hover, focus, and other states</h3>

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

<h3 id="font-size">Font Size</h3>   
Utilities for controlling the font size of an element.

| Class     | Properties                                                |
| --------- | --------------------------------------------------------- |
| text-xs   | font-size: 0.75rem; /12px/ line-height: 1rem; /16px/      |
| text-sm   | font-size: 0.875rem; /14px / line-height: 1.25rem; /20px/ |
| text-base | font-size: 1rem; /16px/ line-height: 1.5rem; /24px/       |
| text-lg   | font-size: 1.125rem; /18px/ line-height: 1.75rem; /28px/  |
| text-xl   | font-size: 1.25rem; /20px/ line-height: 1.75rem; /28px/   |
| text-2xl  | font-size: 1.5rem; /24px/ line-height: 2rem; /32px/       |
| text-3xl  | font-size: 1.875rem; /30px/ line-height: 2.25rem; /36px/  |
| text-4xl  | font-size: 2.25rem; /36px/ line-height: 2.5rem; /40px/    |
| text-5xl  | font-size: 3rem; /48px/ line-height: 1;                   |
| text-6xl  | font-size: 3.75rem; /60px/ line-height: 1;                |
| text-7xl  | font-size: 4.5rem; /72px/ line-height: 1;                 |
| text-8xl  | font-size: 6rem; /96px/ line-height: 1;                   |
| text-9xl  | font-size: 8rem; /128px/ line-height: 1;                  |

Basic usage

#### Setting the font size

Control the font size of an element using the `text-{size}` utilities.

```bash

    <p class="text-xs">
      Lorem ipsum dolor sit amet consectetur adipisicing elit.
      <span class="bg-green-500 text-slate-50 rounded-md px-2">text-xs</span>
    </p>
    <p class="text-sm">
      Lorem ipsum dolor sit amet consectetur adipisicing elit.
      <span class="bg-green-500 text-slate-50 rounded-md px-2">text-sm</span>
    </p>
    <p class="text-base">
      Lorem ipsum dolor sit amet consectetur adipisicing elit.
      <span class="bg-green-500 text-slate-50 rounded-md px-2">text-base</span>
    </p>
    <p class="text-lg">
      Lorem ipsum dolor sit amet consectetur adipisicing elit.
      <span class="bg-green-500 text-slate-50 rounded-md px-2">text-lg</span>
    </p>
    <p class="text-xl">
      Lorem ipsum dolor sit amet consectetur adipisicing elit.
      <span class="bg-green-500 text-slate-50 rounded-md px-2">text-xl</span>
    </p>
    <p class="text-2xl">
      Lorem ipsum dolor sit amet consectetur adipisicing elit.
      <span class="bg-green-500 text-slate-50 rounded-md px-2">text-2xl</span>
    </p>
    <p class="text-3xl">
      Lorem ipsum dolor sit amet consectetur adipisicing elit.
      <span class="bg-green-500 text-slate-50 rounded-md px-2">text-3xl</span>
    </p>
    <p class="text-4xl">
      Lorem ipsum dolor sit amet consectetur adipisicing elit.
      <span class="bg-green-500 text-slate-50 rounded-md px-2">text-4xl</span>
    </p>
    <p class="text-5xl">
      Lorem ipsum dolor sit amet consectetur adipisicing elit.
      <span class="bg-green-500 text-slate-50 rounded-md px-2">text-5xl</span>
    </p>
    <p class="text-6xl">
      Lorem ipsum dolor sit amet consectetur adipisicing elit.
      <span class="bg-green-500 text-slate-50 rounded-md px-2">text-6xl</span>
    </p>
    <p class="text-7xl">
      Lorem ipsum dolor sit amet consectetur adipisicing elit.
      <span class="bg-green-500 text-slate-50 rounded-md px-2">text-7xl</span>
    </p>
    <p class="text-8xl">
      Lorem ipsum dolor sit amet consectetur adipisicing elit.
      <span class="bg-green-500 text-slate-50 rounded-md px-2">text-8xl</span>
    </p>

```

> CHECK `Typography/font-size.html` to see the result.
> Always run this command in your terminal before checking your page.

```bash
    npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch
```

Applying conditionally

<h3 id="font-size-hover-focus">Hover, focus, and other states</h3>

Tailwind lets you conditionally apply utility classes in different states using variant modifiers. For example, use `hover:text-base` to only apply the `text-base` utility on hover.

```bash
    <p class="text-sm hover:text-xl mt-7">HOVER ME!</p>
    <input
      class="text-sm focus:text-8xl mt-7 border-4 border-black"
      placeholder="Click me!"
    />
```

For a complete list of all available state modifiers, check out the [Hover, Focus, & Other States documentation](https://tailwindcss.com/docs/hover-focus-and-other-states).

<h3 id="font-smoothing">Hover, focus, and other states</h3>
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

<h3 style="text-align:center">Font Style</h3>
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
