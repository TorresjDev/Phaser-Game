# Phaser Webpack Template

<<<<<<< HEAD
<<<<<<< HEAD
<<<<<<< HEAD
This is a Phaser 3 project template that uses webpack for bundling. It supports hot-reloading for quick development workflow and includes scripts to generate production-ready builds.

**[This Template is also available as a TypeScript version.](https://github.com/phaserjs/template-webpack-ts)**

### Versions

This template has been updated for:

<<<<<<< HEAD
<<<<<<< HEAD
- [Phaser 3.80.1](https://github.com/phaserjs/phaser)
- [Webpack 5.90.3](https://github.com/webpack/webpack)

![screenshot](screenshot.png)
=======
A Phaser 3 project template with ES6 support via [Babel 7](https://babeljs.io/) and [Webpack 4](https://webpack.js.org/) that includes hot-reloading for development and production-ready builds.
=======
A Phaser 3 project template with ES6 support via [Babel 7](https://babeljs.io/) and [Webpack 5](https://webpack.js.org/) that includes hot-reloading for development and production-ready builds.
>>>>>>> cf1bd0c (Version 2.0.0 of the Project Template)
=======
This is a Phaser 3 project template that uses webpack for bundling. It supports hot-reloading for quick development workflow and includes scripts to generate production-ready builds.
>>>>>>> 4ff2702 (Updated with latest template code and examples. Version 3.0.0.)

### Versions

<<<<<<< HEAD
Loading images via JavaScript module `import` is also supported, although not recommended.
>>>>>>> 017481e (Updated to Phaser 3.50 and ES6 syntax)
=======
This template has been updated for:
>>>>>>> 4ff2702 (Updated with latest template code and examples. Version 3.0.0.)

- [Phaser 3.70.0](https://github.com/phaserjs/phaser)
- [Webpack 5.89.0](https://github.com/webpack/webpack)
=======
- [Phaser 3.80.0](https://github.com/phaserjs/phaser)
=======
- [Phaser 3.80.1](https://github.com/phaserjs/phaser)
>>>>>>> f0e5573 (Phaser 3.80.1)
- [Webpack 5.90.3](https://github.com/webpack/webpack)
>>>>>>> db3b8ab (New Phaser version)

![screenshot](screenshot.png)

## Requirements

[Node.js](https://nodejs.org) is required to install dependencies and run scripts via `npm`.

## Available Commands

| Command | Description |
|---------|-------------|
| `npm install` | Install project dependencies |
<<<<<<< HEAD
<<<<<<< HEAD
| `npm run dev` | Launch a development web server |
| `npm run build` | Create a production build in the `dist` folder |
=======
| `npm start` | Build project and open web server running project |
| `npm run build` | Builds code bundle with production settings (minification, uglification, etc..) into the `dist` folder |
>>>>>>> cf1bd0c (Version 2.0.0 of the Project Template)

## Writing Code

<<<<<<< HEAD
After cloning the repo, run `npm install` from your project directory. Then, you can start the local development server by running `npm run dev`.

The local development server runs on `http://localhost:8080` by default. Please see the webpack documentation if you wish to change this, or add SSL support.

Once the server is running you can edit any of the files in the `src` folder. Webpack will automatically recompile your code and then reload the browser.
=======
After cloning the repo, run `npm install` from your project directory. Then, you can start the local development server by running `npm start`.

After starting the development server with `npm start`, you can edit any files in the `src` folder and webpack will automatically recompile and reload your server (available at `http://localhost:8080` by default).
>>>>>>> 017481e (Updated to Phaser 3.50 and ES6 syntax)

<<<<<<< HEAD
<<<<<<< HEAD
=======
| `npm run dev` | Launch a development web server |
| `npm run build` | Create a production build in the `dist` folder |

## Writing Code

After cloning the repo, run `npm install` from your project directory. Then, you can start the local development server by running `npm run dev`.

The local development server runs on `http://localhost:8080` by default. Please see the webpack documentation if you wish to change this, or add SSL support.

Once the server is running you can edit any of the files in the `src` folder. Webpack will automatically recompile your code and then reload the browser.

>>>>>>> 4ff2702 (Updated with latest template code and examples. Version 3.0.0.)
## Template Project Structure

We have provided a default project structure to get you started. This is as follows:

- `index.html` - A basic HTML page to contain the game.
- `src` - Contains the game source code.
- `src/main.js` - The main entry point. This contains the game configuration and starts the game.
- `src/scenes/` - The Phaser Scenes are in this folder.
- `public/style.css` - Some simple CSS rules to help with page layout.
- `public/assets` - Contains the static assets used by the game.

## Handling Assets

Webpack supports loading assets via JavaScript module `import` statements.

This template provides support for both embedding assets and also loading them from a static folder. To embed an asset, you can import it at the top of the JavaScript file you are using it in:
<<<<<<< HEAD
=======
## Handling Assets

This template provides support for both embedding images and loading them from a static folder. To embed an image, you can import it at the top of the file you are using it in:
>>>>>>> cf1bd0c (Version 2.0.0 of the Project Template)
=======
>>>>>>> 4ff2702 (Updated with latest template code and examples. Version 3.0.0.)

```js
import logoImg from './assets/logo.png'
```

<<<<<<< HEAD
<<<<<<< HEAD
To load static files such as audio files, videos, etc place them into the `public/assets` folder. Then you can use this path in the Loader calls within Phaser:

```js
preload ()
{
    //  This is an example of an imported bundled image.
    //  Remember to import it at the top of this file
    this.load.image('logo', logoImg);

    //  This is an example of loading a static image
    //  from the public/assets folder:
    this.load.image('background', 'assets/bg.png');
}
```

When you issue the `npm run build` command, all static assets are automatically copied to the `dist/assets` folder.

## Deploying to Production

After you run the `npm run build` command, your code will be built into a single bundle and saved to the `dist` folder, along with any other assets your project imported, or stored in the public assets folder.

In order to deploy your game, you will need to upload *all* of the contents of the `dist` folder to a public facing web server.

=======
>>>>>>> af6f938 (Update to 3.24.1.)
=======
To load static files such as images, audio files, videos, etc place them into the `public/assets` folder. Then you can use this path in the Loader calls within Phaser:
=======
To load static files such as audio files, videos, etc place them into the `public/assets` folder. Then you can use this path in the Loader calls within Phaser:
>>>>>>> 4ff2702 (Updated with latest template code and examples. Version 3.0.0.)

```js
preload ()
{
    //  This is an example of an imported bundled image.
    //  Remember to import it at the top of this file
    this.load.image('logo', logoImg);

    //  This is an example of loading a static image
    //  from the public/assets folder:
    this.load.image('background', 'assets/bg.png');
}
```

When you issue the `npm run build` command, all static assets are automatically copied to the `dist/assets` folder.

## Deploying to Production

After you run the `npm run build` command, your code will be built into a single bundle and saved to the `dist` folder, along with any other assets your project imported, or stored in the public assets folder.

In order to deploy your game, you will need to upload *all* of the contents of the `dist` folder to a public facing web server.

>>>>>>> cf1bd0c (Version 2.0.0 of the Project Template)
## Customizing the Template

### Babel

You can write modern ES6+ JavaScript and Babel will transpile it to a version of JavaScript that you want your project to support. The targeted browsers are set in the `.babelrc` file and the default currently targets all browsers with total usage over "0.25%" but excludes IE11 and Opera Mini.

 ```
"browsers": [
  ">0.25%",
  "not ie 11",
  "not op_mini all"
]
 ```

### Webpack
<<<<<<< HEAD

If you want to customize your build, such as adding a new webpack loader or plugin (i.e. for loading CSS or fonts), you can modify the `webpack/config.js` file for cross-project changes, or you can modify and/or create new configuration files and target them in specific npm tasks inside of `package.json`. Please see the [Webpack documentation](https://webpack.js.org/) for more information.

## Join the Phaser Community!

We love to see what developers like you create with Phaser! It really motivates us to keep improving. So please join our community and show-off your work 😄

**Visit:** The [Phaser website](https://phaser.io) and follow on [Phaser Twitter](https://twitter.com/phaser_)<br />
**Play:** Some of the amazing games [#madewithphaser](https://twitter.com/search?q=%23madewithphaser&src=typed_query&f=live)<br />
**Learn:** [API Docs](https://newdocs.phaser.io), [Support Forum](https://phaser.discourse.group/) and [StackOverflow](https://stackoverflow.com/questions/tagged/phaser-framework)<br />
**Discord:** Join us on [Discord](https://discord.gg/phaser)<br />
**Code:** 2000+ [Examples](https://labs.phaser.io)<br />
**Read:** The [Phaser World](https://phaser.io/community/newsletter) Newsletter<br />

Created by [Phaser Studio](mailto:support@phaser.io). Powered by coffee, anime, pixels and love.

The Phaser logo and characters are &copy; 2011 - 2024 Phaser Studio Inc.

All rights reserved.
=======

If you want to customize your build, such as adding a new webpack loader or plugin (i.e. for loading CSS or fonts), you can modify the `webpack/config.js` file for cross-project changes, or you can modify and/or create new configuration files and target them in specific npm tasks inside of `package.json'. Please see the [Webpack documentation](https://webpack.js.org/) for more information.

## Join the Phaser Community!

We love to see what developers like you create with Phaser! It really motivates us to keep improving. So please join our community and show-off your work 😄

<<<<<<< HEAD
If you put the contents of the `dist` folder in a publicly-accessible location (say something like `http://mycoolserver.com`), you should be able to open `http://mycoolserver.com/index.html` and play your game.
>>>>>>> 017481e (Updated to Phaser 3.50 and ES6 syntax)
=======
**Visit:** The [Phaser website](https://phaser.io) and follow on [Phaser Twitter](https://twitter.com/phaser_)<br />
**Play:** Some of the amazing games [#madewithphaser](https://twitter.com/search?q=%23madewithphaser&src=typed_query&f=live)<br />
**Learn:** [API Docs](https://newdocs.phaser.io), [Support Forum](https://phaser.discourse.group/) and [StackOverflow](https://stackoverflow.com/questions/tagged/phaser-framework)<br />
**Discord:** Join us on [Discord](https://discord.gg/phaser)<br />
**Code:** 2000+ [Examples](https://labs.phaser.io)<br />
**Read:** The [Phaser World](https://phaser.io/community/newsletter) Newsletter<br />

Created by [Phaser Studio](mailto:support@phaser.io). Powered by coffee, anime, pixels and love.

The Phaser logo and characters are &copy; 2011 - 2024 Phaser Studio Inc.

All rights reserved.
>>>>>>> 4ff2702 (Updated with latest template code and examples. Version 3.0.0.)
