# Softnanolab Group Website

This will be our new website repository!

# tailwind

Using https://tailwindcss.com/docs/installation

- Setup by going `npm install tailwindcss@latest postcss@latest autoprefixer@latest`
- `"build-css": "tailwindcss build src/styles.css -o softnanoweb/styles.css"` in the scripts part of package.json will process the css
- run using `npm run build-css`

# Package.json

```
  "scripts": {
    "deploy": "gh-pages -d softnanoweb"
  },
```

This deploys the pages inside `softnanoweb` onto the gh-pages branch of the repo. There must be a file called `index.html` in here btw...

## Deploy

After pushing... use the command `npm run deploy` and that should deploy the page
