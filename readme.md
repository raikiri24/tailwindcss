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
   <span style="background-color: rgba(51, 110, 176, 0.5)"> `content: ["./src/**/*.{html,js}"]` </span>
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

## WE'RE NOW GOOD TO GO!

#### LET'S NOW EXPLORE HOW TO USE TAILWIND IN OUR PROJECTS
