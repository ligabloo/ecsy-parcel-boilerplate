# ECSY Parcel Boilerplate

A simple boilerplate project for using [ECSY](https://ecsy.io) with [Parcel](https://v2.parceljs.org/).

Directly inspired by [`MozillaReality/ecsy-webpack-boilerplate`](https://github.com/MozillaReality/ecsy-webpack-boilerplate).

[View Live Demo](https://ligabloo.github.io/ecsy-parcel-boilerplate/)

## Downloading

We recommend [`degit`](https://github.com/Rich-Harris/degit) for simply scaffolding the project:
```
npm i -g degit
```

After this, you only need to run the following command to download the boilerplate:
```
degit ligabloo/ecsy-parcel-boilerplate#main [your-desired-project-name]
```

Degit will ensure to download only the latest commit on the `main` branch, without carrying the entire Git repository's history.

**Note**: this also means that your project won't have a Git repo initialized! You you'd like to use it for source control, make sure to run `git init` before starting your work.

## Developing

To get started, install the included dependencies:

```
npm install
```

Then, run the start script:

```
npm start
```

This will make Parcel start a local development server on your machine. The console will output the localhost URL for opening the page on your browser - the default link should be http://localhost:1234.

## Building
To build a production ready bundle, simply run:

```
npm run build
```

The bundled code will be output to the `/dist` directory.

## Deploying

If you're hosting your project on GitHub, you may deploy your build to a GitHub Pages instance. Since this project includes the `gh-pages` npm script, it should be as simple as:
  - building your project
  - making sure your git repository has a remote URL to a GitHub repository
  - running the following command:
```
npm run deploy
```
This will automatically create a branch name `gh-pages` to your repository, copy all the files from the `dist` folder to it, commit them and push the changes to GitHub. See the [`gh-pages` npm script page](https://www.npmjs.com/package/gh-pages) for more info.
