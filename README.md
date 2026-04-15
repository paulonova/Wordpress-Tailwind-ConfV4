# Wordpress com configuracao do TailwindCss v4

## SETTINGS

* Install Tailwindcss/cli

```
npm install tailwindcss @tailwindcss/cli

```

* Create a src/input.css  and write:

```
/*
Theme Name: Name of theme
Description: A description here
Version: 1.0
Author: Paulo Vila Nova
*/

@import "tailwindcss";
@config "../tailwind.config.js";

```

* In package.json write the script to run the css from Tailwind:

```
"scripts": {
    "build-css": "npx tailwindcss -i ./src/input.css -o ./style.css --watch",
  },

```


* Google Material Symbols

<a href="https://fonts.google.com/icons">Link to Google Material</a>

- In functions.php set the style:

```
wp_enqueue_style('google-material-symbols', '//fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&display=swap');
```


### Instructions

* De uma boa olhada no projeto e configure corretamente senao nao ira funcionar.