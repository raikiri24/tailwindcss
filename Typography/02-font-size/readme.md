#### Typography

- [Font Size](#font-size)
- [Font Size Hover, focus, and other states](#font-size-hover-focus)

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
