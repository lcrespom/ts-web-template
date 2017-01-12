# ts-web-template
A template for quickly starting up a web project based on TypeScript.

It provides the following `npm run` commands:
- `start`, `serve`: Launches a small server for testing at http://localhost:8080. Live-reload is enabled, so any changes in the `web/` directory will trigger a page reload.
- `build`: Builds the TypeScript code from `src/main.ts` and all its dependencies, bundles it through Browserify and places the bundle and map files in the `web/` directory.
- `watch`: Watches for any changes in `src/**/*.ts` and runs `npm build` in case any change is detected.

It also provides the following configuration files with useful defaults that can be adapted to your own preferences:
- `.gitignore`: the usual files to be ignored
- `tsconfig.json`: TypeScript configuration. Notice that the JS target version is set to `ES6`, because all modern browsers already support it. If you need to support older browsers, change the `target` property to `ES5`.
- `tslint.json`: TypeScript linter rules
- `.editorconfig`: Editor settings
- `package.json`: Project manifest => must be changed in order to adapt to user's project

After the template is installed and adapted, you can replace this `README.md` file with the proper main project document.

## Installation
1. Clone this repository.
2. Rename its directory to your project's name.
3. Remove the .git directory and then run `git init`.
4. Modify `package.json`, changing at least the `name`, `description` and `repository` properties.
5. Run `npm install`.
6. You are ready to go.
