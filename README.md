# Installation of Vite

- npm create vite@latest

# Installation of Tailwind CSS with PostCSS

https://tailwindcss.com/docs/installation/using-postcss

- npm install -D tailwindcss postcss autoprefixer
- npx tailwindcss init

## Add to style.css file

- @tailwind base;
- @tailwind components;
- @tailwind utilities;

## Installation of prettier

- npm install --save-dev prettier
- - test prettier: npx prettier -c src/\*_/_.js

## Installation of ESLint

- npx eslint --init

✔ How would you like to use ESLint? · problems

✔ What type of modules does your project use? · esm

✔ Which framework does your project use? · none

✔ Does your project use TypeScript? · No

✔ Where does your code run? · browser

✔ What format do you want your config file to be in? · JSON

## Installation of mrm (lint-staged)

- npx mrm@2 lint-staged
- Add to package.json file:
  "lint-staged": {
  "_.js": [
  "eslint --fix",
  "prettier --write"
  ],
  "_.html": [
  "prettier --write"
  ],
  "\*.scss": [
  "prettier --write"
  ]
  }
