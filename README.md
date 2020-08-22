# IDE Extensions

> A repository with my extensions for the IDEs I use

## Visual Studio Code

At the moment, VS Code is my favorite IDE, so I started this project with him

### settings.json

In this file are my VS Code settings.

To modify the VS Code settings press: `Ctr + LShift + P` and select `Preferences: Open Settings (JSON)`

Copy the content of the file in this repository to the file that will open.

### Darguima Snippets

Includes snippets for JS, JSX, TS, TPX, CSS;

#### JS and JSX

|    prefix    |     description                                  |
|--------------|--------------------------------------------------|
|        `rfc` | Create a basic ReactJS functional component      |


#### TS and TSX

|    prefix    |     description                                  |
|--------------|--------------------------------------------------|
|        `rfc` | Create a basic ReactJS functional component      |


#### CSS

|    prefix    |     description                                  |
|--------------|--------------------------------------------------|
|        `rfc` | Create a initial CSS file to a basic RFC         |
|        `ncs` | Create a new CSS object                          |
|       `nfcs` | Create a new CSS object with flex properties     |
|        `fps` | Add flex properties to the CSS object            |


#### Installation

To install these snippets follow the next steps.

1. Go to the root folder of the extension (IDE-Extensions/VSCode/darguima-snippets/)

2. > npm install -g vsce

3. > vsce package

4. > code --install-extension darguima-snippets-${snippet version}.vsix

##### Notes

* Make sure that Node JS is already installed (to use npm);

* Change $ {snippet version} to the current version of the snippet (only copy the file name);

* If you want you can use the package that was previously included in the folder


### Darguima Theme

A high contrast theme to VS Code based in Monokai Charcoal (gray).

#### Installation

To install this theme follow the next steps.

1. Go to the root folder of the extension (IDE-Extensions/VSCode/darguima-theme/)

2. > npm install -g vsce

3. > vsce package

4. > code --install-extension darguima-theme-${theme version}.vsix

##### Notes

* Make sure that Node JS is already installed (to use npm);

* Change $ {theme version} to the current version of the theme (only copy the file name);

* If you want you can use the package that was previously included in the folder

## nodejsSetup.md

* A markdown file with the steps to create a basic setup to create a server with node

* Yes, I know that isn't a extension but I want put it on the Git Hub so I choose this repository
