# RosettaLab
Generic sensor application designed to quickly connect to a sensor and read back its data


## Electron Setup
Follow instructions from https://www.electronjs.org/docs/latest/tutorial/quick-start

1. Install node and npm

        node -v
        npm -v

2. Create a new folder for our project and initialize it with npm


    mkdir my-electron-app && cd my-electron-app
    npm init

Entry point is main.js

package.json should look like this

    {
        "name": "my-electron-app",
        "version": "1.0.0",
        "description": "Hello World!",
        "main": "main.js",
        "author": "Jane Doe",
        "license": "MIT"
    }

Install electron and it's dev dependencies

    npm install --save-dev electron

To execute electron add the following to package.json

    {
        "scripts": {
            "start": "electron ."
        }
    }

3. Setup main.js, index.html, and preload.js as per instructions

4. Start electron app using

    npm start

5. Setup application to be distributed using Electron Forge

    npm install --save-dev @electron-forge/cli
    npx electron-forge import

6. Create distributable using

    npm run make

This will be found in the out/ folder