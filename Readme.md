# Installation

## Install Tailwind CSS

Install `tailwindcss` via npm, and create your `tailwind.config.js file`.

```sh
npm install -D tailwindcss
npx tailwindcss init
```

## Configure your template paths

Add the paths to all of your template files in your `tailwind.config.js` file.

```sh
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js}"],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

## Add the Tailwind directives to your CSS

Add the `@tailwind` directives for each of Tailwind’s layers to your main CSS file.

```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

## Start using Tailwind in your HTML
Add your compiled CSS file to the `<head>` and start using Tailwind’s utility classes to style your content.

```html
<!doctype html>
<html>
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link href="./output.css" rel="stylesheet">
</head>
<body>
  <h1 class="text-3xl font-bold underline">
    Hello world!
  </h1>
</body>
</html>
```

## Start the Tailwind CLI build process
Run the CLI tool to scan your template files for classes and build your CSS.

```sh
npx tailwindcss -i ./src/input.css -o ./src/output.css --watch
```

## Rise the Live Server
In vscode you must rise the live server at the end of the process.

## External Sources

[instalar TAILWIND CSS V3 Facil](https://www.youtube.com/watch?v=PcrTJS9mWKY&ab_channel=JUANRAMONCORNEJO)
