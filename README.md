composer create-project laravel/laravel:^9.0 laravel-movies-example

npm install -D tailwindcss postcss autoprefixer

npx tailwindcss init

In your webpack.mix.js file, add tailwindcss as a PostCSS plugin.
mix.js("resources/js/app.js", "public/js")
  .postCss("resources/css/app.css", "public/css", [
    require("tailwindcss"),
  ]);



Add the paths to all of your template files in your tailwind.config.js file.
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: [
    "./resources/**/*.blade.php",
    "./resources/**/*.js",
    "./resources/**/*.vue",
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}




Add the @tailwind directives for each of Tailwind’s layers to your ./resources/css/app.css file.
@tailwind base;
@tailwind components;
@tailwind utilities;



npm run watch


https://laravel-livewire.com/docs/2.x/installation
composer require livewire/livewire


https://github.com/aniftyco/tailwindcss-spinner
npm install --save-dev tailwindcss-spinner

https://github.com/alpinejs/alpine/tree/v2.8.2


https://github.com/spatie/laravel-view-models


https://infinite-scroll.com/
