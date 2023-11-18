![](https://github.com/SergeyDavidovich/BlazorWithTailwind/blob/master/blazor-tailwind.png)
----
## Project description ##
### The project is Blazor and TailwindCSS CLI tools installation for Visual Studio Wasm standalone project template ###
---
## 1. Prerequisites ##
### Create new Blazor Wasm project in Visual Studio ###
### Install Tailwind CSS ###
Open in terminal project folder (the folder where the .csproj file is located)
```
npm install -D tailwindcss 
npx tailwindcss init
````

## 2. File structure and configuration 
### File structure
```
project folder (the folder where the .csproj file is located)
    tailwind.config.js
        Styles/tailwind.css
        wwwroot/dist/tailwind.css
```
### File content - wwwroot/input/input.css
```
@tailwind base;
@tailwind components;
@tailwind utilities;
```
### File content - tailwind.config.js
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
### File content- index.html
```
    <base href="/" />
    <link href="dist/tailwind.css" rel="stylesheet" />
```
## 3. Terminal compilation string
#### npx tailwindcss -i ./Styles/tailwind.css -o ./wwwroot/dist/tailwind.css --watch ####
## 4. Project links
- [Installation - Tailwind CSS](https://tailwindcss.com/docs/installation)
- [Adding Tailwind CSS v3 to a Blazor app](https://chrissainty.com/adding-tailwind-css-v3-to-a-blazor-app/)
- [Using Tailwind Css With .Net Blazor](https://dev.to/rasheedmozaffar/using-tailwind-css-with-net-blazor-4ng7)

