# NodeJS Setup

> yarn init -y

> yarn add typescript -D

> echo "node_modules" > .gitignore
> echo "dist" >> .gitignore

> yarn tsc --init

> mkdir src

> touch src/server.ts

> yarn add ts-node-dev -D

> Add the following object to the _package.json_

`
"scripts": {
    "dev": "ts-node-dev --respawn --transpile-only --ignore-watch node_modules --no-notify src/server.ts"
  },
`

On _tsconfig.json_

> "target": "es2017",

> "lib": ["ES6"],
> "allowJs": true,

> "outDir": "./dist",
> "rootDir": "./src",

> "removeComments": true,

> // "strict": true,

> "typeRoots": [
      "./node_modules/@types",
      "./src/@types"
    ],

> "resolveJsonModule": true,

> "baseUrl": ".",
> "paths": {"@name_path/*": ["./src/path/path/name_path/*"]},

Terminal: 

> yarn add tsconfig-paths -D

> Change the following object on the _package.json_

`
"scripts": {
    "dev": "ts-node-dev -r tsconfig-paths/register --respawn --transpile-only --ignore-watch node_modules --no-notify src/server.ts"
  },
`

Terminal: 

> yarn eslint --init

Select:

> "To check syntax, find problems, and enforce code style"

> "JavaScript modules (import/export)"

> "None of these"

> "Yes"

> "node" (press Space to unselect "Browser")

> "Use a popular style guide"

> "Standard: https://github.com/standard/standard"

> "JSON"

> "No" (for the yarn)

Copy the dependencies

> yarn add ${dependencies} -D

Install the ES Lint Extension

In settings.json (of VS Code) add the object:

`"editor.codeActionsOnSave": {
  "source.fixAll.eslint": true
}`

Create .eslintignore and add:

> dist
> /*.js


Terminal: 

> yarn add @babel/cli @babel/core @babel/node @babel/ preset-env @babel/preset-typescript babel-plugin-module-resolver -D


Create a file _babel.config.js_ and add:

"""

module.exports = {
  presets: [
    [
      '@babel/preset-env',
      {
        targets: {
          node: 'current'
        }
      }
    ],
    '@babel/preset-typescript'
  ],

  plugins: [
    ['module-resolver', {
      alias: {
        '@name_path': './src/path/path/name_path'
      }
    }]
  ],

  ignore: [
  ]
}


"""

> Change the following object on the _package.json_

`
"scripts": {
    "build": "babel src --extensions \".js,.ts\" --out-dir dist --copy-files --no-copy-ignored",

    "start": "node dist/server.ts",

    "dev": "ts-node-dev -r tsconfig-paths/register --respawn --transpile-only --ignore-watch node_modules --no-notify src/server.ts"
  },
`


