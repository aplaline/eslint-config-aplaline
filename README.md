## ESLint configuration for Aplaline projects

### Usage

In ```package.json``` add the following to configure eslint:

```
  "devDependencies": {
    "eslint": "^4.19.1",
    "eslint-config-aplaline": "git+https://github.com/aplaline/eslint-config-aplaline#1.5.3",
  },
  "eslintConfig": {
    "extends": [
      "eslint-config-aplaline"
    ]
  }
```

To get Visual Studio Code to show warnings create ```.vscode/settings.json``` with the following content:

```
{
  "eslint.validate": [
    "javascript",
    "javascriptreact",
    "vue"
  ]
}
```

Additionally it is advised to set the following additional settings in ```.vscode/settings.json```:

```
{
  "editor.lineNumbers": "on",
  "beautify.tabSize": 2,
  "beautify.options": {
    "indent_size": 2
  }
}
```
