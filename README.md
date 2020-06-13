It provides an initial structure for setting up a development environment for React using the airbnb style guide, eslint, prettier and Visual Studio code.

## Environment

### Visual Studio Plugins
Let's check it out the list of required Visual Studio plugins to enable the eslint and code formatting conventions.

#### ESLint for Visual Studio Code

You can find it here: [EsLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)

#### Prettier - Code formatter

You can find it here: [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)

#### EditorConfig for Visual Studio Code

You can find it here: [EditorConfig](https://marketplace.visualstudio.com/items?itemName=EditorConfig.EditorConfig)

#### Default Formatter

To ensure that this extension is used over other extensions you may have installed, be sure to set it as the default formatter in your VS Code settings.

`Ctrl+Shift+P -> Setting -> Preferences: Open Settings (JSON)`

```json
    "[javascript]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode",
        "editor.formatOnSave": true,
        "editor.codeActionsOnSave": {
            "source.fixAll.eslint": true
        }
    },
    "[javascriptreact]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode",
        "editor.formatOnSave": true,
        "editor.codeActionsOnSave": {
            "source.fixAll.eslint": true
        }
    },
```


### Dev dependencies


```json
    "devDependencies": {
      "eslint": "^6.6.0",
      "eslint-config-airbnb": "^18.1.0",
      "eslint-config-prettier": "^6.11.0",
      "eslint-plugin-import": "^2.21.2",
      "eslint-plugin-prettier": "^3.1.3",
      "eslint-plugin-react": "^7.20.0",
      "eslint-plugin-react-hooks": "^4.0.4",
      "prettier": "^2.0.5",
      "prettier-eslint": "^11.0.0"
    }
```

### Config files

### `.eslintrc.json` File to set up the eslint/prettier conventions.

### `.eslintrc.json` File to set up the source code path for enabling the absolute path import.


### File structure
    .
    ├── public
    ├── src
    │   ├── common
    │   ├── components
    |   |    ├── container
    |   |    ├── presentational
    |   |    ├── pages
    │   ├── contexts
    │   ├── reducers
    │   ├── styles
    └── .editorconfig
    └── .eslintrc.json
    └── .gitignore
    └── jsconfig.json
    └── package.json
    └── README.md


## Available Scripts

In the project directory, you can run:

### `yarn start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.

### `yarn test`

Launches the test runner in the interactive watch mode.<br />
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `yarn build`

Builds the app for production to the `build` folder.<br />
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br />
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.


## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).
