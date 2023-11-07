![](https://github.com/SergeyDavidovich/BlazorWithTailwind/blob/master/blazor-tailwind.png)
----
## Project description ##
### The project is Blazor and TailwindCSS CLI tools installation for visual Studio Wasm standalone project template ###
---
## File structure and configuration 
### File structure
```
project folder - BlazorWithTailwind (for this solution only)
    tailwind.config.js
        Styles/tailwind.css
        wwwroot/dist/tailwind.css
```
### File - wwwroot/input/input.css
```
@tailwind base;
@tailwind components;
@tailwind utilities;
```
### File - tailwind.config.js
```
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ['./**/*.{razor,html}'],
  theme: {
    extend: {},
  },
  plugins: [],
}
```
### File - index.html
```
    <base href="/" />
    <link href="dist/tailwind.css" rel="stylesheet" />
```
## Terminal compilation string
#### npx tailwindcss -i ./Styles/tailwind.css -o ./wwwroot/dist/tailwind.css --watch ####
## Project links
- [Installation - Tailwind CSS](https://tailwindcss.com/docs/installation)
- [Adding Tailwind CSS v3 to a Blazor app](https://chrissainty.com/adding-tailwind-css-v3-to-a-blazor-app/)
- [Using Tailwind Css With .Net Blazor](https://dev.to/rasheedmozaffar/using-tailwind-css-with-net-blazor-4ng7)

