# Softnanolab Group Website

This will be our new website repository! It is currently being hosted here: https://softnanolab.github.io/softnanoweb/

# tailwind

Using https://tailwindcss.com/docs/installation

- Setup by going `npm install tailwindcss@latest postcss@latest autoprefixer@latest`
- `"build-css": "tailwindcss build src/styles.css -o softnanoweb/styles.css"` in the scripts part of package.json will process the css
- run using `npm run build-css`

## customising tailwind classes

Firstly create a `tailwind.config.js` file using `npx tailwindcss init --full`, which creates a config file including **all** the default values.

Now rename this to `tailwind-default.config.js` file (FOR REFERENCE) and then run the same command without the --full flag: `npx tailwindcss init`

Whenever a default value is changed (not recommended), or new value is added (the way to do it...), just re-execute `npm run build-css` (i.e. that from package.json file) in the terminal! Make sure you are in the base directory of the repo!

# Package.json

```
  "scripts": {
    "deploy": "gh-pages -d softnanoweb"
  },
```

This deploys the pages inside `softnanoweb` onto the gh-pages branch of the repo. There must be a file called `index.html` in here btw...

## Deploy

After pushing... use the command `npm run deploy` and that should deploy the page

## Locally deploying

Use live server vscode extension!
