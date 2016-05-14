###App
Basic skeleton forked from [electron-quick-start](https://github.com/electron/electron-quick-start)

React code written in *ES6* & *JSX*, and transpiled using *babel*


###Setup
1. `cd` into the project folder
2. add images with the following relative URLs
   * `public/img/logo.png`
   * `public/img/soundcloud.png`

3. add your soundcloud cliend ID in the file `app/containers/app.container.js`
  * replace `YOUR_SOUNDCLOUD_CLIENT_ID` with your client ID

4. run `npm install`

5. run these 2 commands simultaneously(in different terminal )-
  * `npm run watch` - to make `public/js/bundle.js` again on every js change
  * `npm start` - to start and live-reload the electron app on every change

###Minor Changes from the tutorial to make it all work
* `npm install watchify --save` to add watchify in the package.json as it is required to run watch
* Wrapping `"presets": ["es2015", "react"]` in `{}` to make valid `.babelrc`
* `"use strict";` on top of the `main.js` to prevent const, let errors
* different `electron-reload` require in `main.js`-
```js
require('electron-reload')(__dirname, {
  electron: require('electron-prebuilt')
});
```

###Tutorial App ([scotch.io](https://scotch.io))

Link to the tutorial-
[Part 1](https://scotch.io/tutorials/build-a-music-player-with-react-electron-i-setup-basic-concepts),
[Part 2](https://scotch.io/tutorials/build-a-music-player-with-react-electron-ii-making-the-ui),
[Part 3](https://scotch.io/tutorials/build-a-music-player-with-react-electron-iii-bringing-it-all-together)
