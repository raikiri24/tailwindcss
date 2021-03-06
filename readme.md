<h1 style="text-align: center"><a href="https://tailwindcss.com/docs/installation">Tailwind Installation</a></h1>

## LET'S GET STARTED

Tailwind CLI

1. Install Tailwind CSS.
   Install `tailwindcss` via npm by typing in your terminal this command:

`npm install -D tailwindcss`

To create your `tailwind.config.js` type:

`npx tailwindcss init`

2. Configure your template paths
   In your `tailwind.config.js` file add the path of your template files.

   `root folder > tailwind.config.js` (directory)

   Add this line inside the module.exports

   `module.exports = {`
   <span style="background-color: rgba(51, 110, 176, 0.5)"> `content: ["./**/*.{html,js}"]` </span>
   `theme: { extend: {}, }, plugins: [], }`

3. Create a folder named `src` then create a stylesheet named `input`.

   Your directory should look like this.

   > -root folder  
   > &nbsp;&nbsp;&nbsp;-src  
   > &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;-input.css  
   > &nbsp;&nbsp;&nbsp;-index.html

4. Add the Tailwind directives to your CSS  
   Add the `@tailwind` directives for each Tailwind's layers to your main CSS file.

   `root folder > src > input.css` (directory)

   > ```bash
   >  @tailwind base;
   >  @tailwind components;
   >  @tailwind utilities;
   > ```

5. Start the Tailwind CLI build process  
   Run the CLI tool to scan your template files for classes and build your CSS

   ```bash
    npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch
   ```

6. Start using Tailwind in your HTML
   Add your compile CSS file to the `<head>` and start using Tailwind's utility classes to style your content.

   ```bash
   <!DOCTYPE html>
       <html lang="en">
       <head>
           <meta charset="UTF-8" />
           <meta http-equiv="X-UA-Compatible" content="IE=edge" />
           <meta name="viewport" content="width=device-width, initial-scale=1.0" />
           <title>Document</title>
           <link href="./dist/output.css" />
       </head>
   ```

WE'RE NOW GOOD TO GO!

LET'S NOW EXPLORE HOW TO USE TAILWIND IN OUR PROJECTS

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
