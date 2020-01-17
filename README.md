# Automagically have a common code quality for React / JS

## Setup Eslint with Airbnb Style Guide

### Install Eslint

`npm i -D eslint eslint-config-airbnb eslint-plugin-import eslint-plugin-jsx-a11y eslint-plugin-react`

### Install Prettier

`npm i -D prettier-eslint-cli eslint-config-prettier`

### Install Husky

`npm i -D husky lint-staged`

### Create .eslintrc file in the root directory next to package.json

<pre>{
    "env": { "browser": true }, 
    "extends": ["airbnb", "prettier"] 
}</pre>

### Install VSCode extentions

Launch extension installation by pressing CMD+P

`ext install dbaeumer.vscode-eslint`

`ext install esbenp.prettier-vscode`

### Edit settings.json for VSCode to have these options

<pre>
    "editor.formatOnPaste": true,
    "editor.formatOnSave": true,
    "editor.formatOnType": true,
    "javascript.format.enable": true,
    "editor.codeActionsOnSave": {
        // For JSLint
        "source.fixAll.jslint": true,
        // For ESLint
        "source.fixAll.eslint": true,
        // For TSLint
        "source.fixAll.tslint": true,
        // For Stylelint
        "source.fixAll.stylelint": true
    }
</pre>
