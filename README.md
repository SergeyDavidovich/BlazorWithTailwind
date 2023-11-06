![](https://github.com/SergeyDavidovich/BlazorWithTailwind/blob/master/BlazorTailwind.png)
----
## Project description ##
### The project is Blazor WASM + TailwindCSS CLI tools installation for visual Studio Wasm project alone template ###
---
## Configuration and file structure

### File structure
```
project folder - BlazorWithTailwind (in this solution only)
  wwwroot
    input --> input.css
    output --> output.css
  tailwind.css
```
### File - wwwroot/src/tailwind.css
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
    <link href="css/tailwind.css" rel="stylesheet" />
```
## Terminal compilation string
npx tailwindcss -i ./Styles/tailwind.css -o ./wwwroot/css/tailwind.css --watch
## Project links
- [Installation - Tailwind CSS](https://tailwindcss.com/docs/installation)
- [Adding Tailwind CSS v3 to a Blazor app](https://chrissainty.com/adding-tailwind-css-v3-to-a-blazor-app/)
- [Using Tailwind Css With .Net Blazor](https://dev.to/rasheedmozaffar/using-tailwind-css-with-net-blazor-4ng7)

