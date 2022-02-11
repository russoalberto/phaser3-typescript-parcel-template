# Phaser 3 + TypeScript + Parcel 2 Template

![License](https://img.shields.io/badge/license-MIT-green)

This is a fork of [phaser3-typescript-parcel-template](https://github.com/ourcade/phaser3-typescript-parcel-template).

## Getting Started

Clone this repository to your local machine:

```bash
git clone https://github.com/russoalberto/phaser3-typescript-parcel2-template.git
```

This will create a folder named `phaser3-typescript-parcel2-template`. You can specify a different folder name like this:

```bash
git clone https://github.com/russoalberto/phaser3-typescript-parcel2-template.git my-folder-name
```

Go into your new project folder and install dependencies:

```bash
cd phaser3-typescript-parcel2-template # or 'my-folder-name'
npm install
```

Start development server:

```
npm run start
```

To create a production build:

```
npm run build
```

Production files will be placed in the `dist` folder. Then upload those files to a web server.

## Project Structure

```
    .
    ├── dist
    ├── node_modules
    ├── public
    ├── src
    │   ├── scenes
    │   │   ├── MainScene.ts
    │   ├── index.html
    │   ├── main.ts
    ├── package.json
```

The contents of this template is the basic [Phaser 3 getting started example](http://phaser.io/tutorials/getting-started-phaser3/part5).

This template assumes you will want to organize your code into multiple files and use TypeScript.

TypeScript files are intended for the `src` folder. `main.ts` is the entry point referenced by `index.html`.

Other than that there is no opinion on how you should structure your project. There is a `scenes` folder in `src` where the `MainScene.ts` lives but you can do whatever you want.

## Static Assets

Any static assets like images or audio files should be placed in the `public` folder. It'll then be served at http://localhost:8000/assets/images/my-image.png

Example `public` structure:

```
    public
    ├── assets
    │   ├── images
    │   ├── my-image.png
    │   ├── music
    │   ├── ...
    │   ├── sfx
    │   ├── ...
```

They can then be loaded by Phaser with `this.image.load('my-image', 'assets/images/my-image.png')`.
