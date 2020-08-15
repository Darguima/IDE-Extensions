# Visual Studio Code

At the moment, VS Code is my favorite IDE, so I started this project with him

## Darguima Snippets

Includes snippets for JS, JSX, TS, TPX, CSS;

### JS and JSX

|    prefix    |     description                                  |
|--------------|--------------------------------------------------|
|        `rfc` | Create a basic ReactJS functional component      |


### TS and TSX

|    prefix    |     description                                  |
|--------------|--------------------------------------------------|
|        `rfc` | Create a basic ReactJS functional component      |


### CSS

|    prefix    |     description                                  |
|--------------|--------------------------------------------------|
|        `rfc` | Create a initial CSS file to a basic RFC         |
|        `ncs` | Create a new CSS object                          |
|       `nfcs` | Create a new CSS object with flex properties     |
|        `fps` | Add flex properties to the CSS object            |


### Installation

To install these snippets follow the next steps.

1. Go to the root folder of the extension (IDE-Extensions/VSCode/darguima-snippets/)

2. > npm install -g vsce

3. > vsce package

4. > code --install-extension darguima-snippets-${snippet version}.vsix

#### Notes

* Make sure that Node JS is already installed (to use npm);

* Change $ {snippet version} to the current version of the snippet (only copy the file name);

* If you want you can use the package that was previously included in the folder
