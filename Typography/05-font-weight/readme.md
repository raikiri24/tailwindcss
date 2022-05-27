#### Typography

- [Font Weight](#font-weight)
- [Font Style Hover, focus and other states](#font-weight-hover-focus-states)

<h3 style="text-align:center" id="font-weight">Font Weight</h3>
Utilities for controlling the font weight of an element.

| Class           | Properties        |
| --------------- | ----------------- |
| font-thin       | font-weight: 100; |
| font-extralight | font-weight: 200; |
| font-light      | font-weight: 300; |
| font-normal     | font-weight: 400; |
| font-medium     | font-weight: 500; |
| font-semibold   | font-weight: 600; |
| font-bold       | font-weight: 700; |
| font-extrabold  | font-weight: 800; |
| font-black      | font-weight: 900; |

Basic usage
​
Setting the font weight
Control the font weight of an element using the font-{weight} utilities.

```bash

    <p class="font-thin">
      Lorem ipsum dolor sit amet consectetur adipisicing elit.
      <span class="bg-green-500 text-slate-50 rounded-md px-2">font-thin</span>
    </p>
    <p class="font-extralight">
      Lorem ipsum dolor sit amet consectetur adipisicing elit.
      <span class="bg-green-500 text-slate-50 rounded-md px-2"
        >font-extralight</span
      >
    </p>
    <p class="font-light">
      Lorem ipsum dolor sit amet consectetur adipisicing elit.
      <span class="bg-green-500 text-slate-50 rounded-md px-2">font-light</span>
    </p>
    <p class="font-normal">
      Lorem ipsum dolor sit amet consectetur adipisicing elit.
      <span class="bg-green-500 text-slate-50 rounded-md px-2"
        >font-normal</span
      >
    </p>
    <p class="font-medium">
      Lorem ipsum dolor sit amet consectetur adipisicing elit.
      <span class="bg-green-500 text-slate-50 rounded-md px-2"
        >font-medium</span
      >
    </p>
    <p class="font-semibold">
      Lorem ipsum dolor sit amet consectetur adipisicing elit.
      <span class="bg-green-500 text-slate-50 rounded-md px-2"
        >font-semibold</span
      >
    </p>
    <p class="font-bold">
      Lorem ipsum dolor sit amet consectetur adipisicing elit.
      <span class="bg-green-500 text-slate-50 rounded-md px-2">font-bold</span>
    </p>
    <p class="font-extrabold">
      Lorem ipsum dolor sit amet consectetur adipisicing elit.
      <span class="bg-green-500 text-slate-50 rounded-md px-2"
        >font-extrabold</span
      >
    </p>
    <p class="font-black">
      Lorem, ipsum dolor sit amet consectetur adipisicing elit.
      <span class="bg-green-500 text-slate-50 rounded-md px-2">font-black</span>
    </p>
```

Applying conditionally
​

<h3 style="text-align:center" id="font-weight-hover-focus-states"> Hover, focus, and other states </h3>

Tailwind lets you conditionally apply utility classes in different states using variant modifiers. For example, use `hover:font-bold` to only apply the `font-bold` utility on hover.

```bash

    <h1 class="mt-7 font-bold text-3xl">
      FONT WEIGHT HOVER,FOCUS and OTHER STATE
    </h1>
    <br />
    <p class="font-bold hover:font-thin">Hover me!</p>
    <br />
    <input
      type="text"
      name=""
      id=""
      class="border-4 border-black font-normal focus:font-extrabold"
      placeholder="Click me!"
    />

```

For a complete list of all available state modifiers, check out the [Hover, Focus, & Other States documentation](https://tailwindcss.com/docs/hover-focus-and-other-states).
