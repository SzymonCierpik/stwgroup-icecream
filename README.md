# parcel-project-template

## Dependencies
You need to have the LTS version of Node.js installed on your computer.

```shell
npm ci
```

## Development
Start the development server.

```shell
npm run dev
```


### Praca

Włączyć tryp pracy.

```shell
npm run dev
```

Open your browser and go to [http://localhost:1234](http://localhost:1234) to view the project.

## Deployment
The code will automatically build and deploy the current version of the project to GitHub Pages, specifically the gh-pages branch, whenever changes are made to the main branch. For example, after a direct push or when a pull request is merged. To make this work, you need to modify the homepage field and the build script in the package.json file, replacing username and repository-name with your own.

```json
"homepage": "https://username.github.io/repository-name",
"scripts": {
  "build": "parcel build src/*.html --public-url /repository-name/"
},
},
```
After some time, you will be able to see the live website at the URL specified in the updated homepage property, for example, https://username.github.io/repository-name.

## Files and Folders
All style partials should be located in the src/sass folder and imported into src/sass/main.scss.
Add images to the src/images folder, and make sure to optimize them before adding. The build process simply copies the used images to avoid optimizing them each time, as it can be time-consuming on slower computers.
