## Open Your Terminal (OSX) or Powershell (Windows)

## Make a Project Directory

## Setup Project

`yarn init`

## Install `Next.js`

`yarn add next ramda`

## Open This Folder with `Code`

To open the current directory using your terminal, type the following:

`code .`

Alternatively, open the `Code` app the `File->Open Folder` to select
your folder.

## Add a `dev` Script

Open `package.json`

Add the following:
```json
  "scripts": {
    "dev": "next"
  },
```

[At the end of this page](#run-the-project), you will run `yarn run dev` to trigger this 
script to run "next" in our project. But not yet!

Your `package.json` should now look like:
```json
{
  "name": "hangman",
  "version": "1.0.0",
  "main": "index.js",
  "license": "MIT",
  "scripts": {
    "dev": "next"
  },
  "dependencies": {
    "next": "^1.2.3",
    "ramda": "^0.23.0"
  }
}
```

## Create a JavaScript File
In code, create a folder called `pages`

> Right-click, "New Folder", name it "pages"

Then create an `index.js` file in the `pages` folder.

> Right-click the "pages" folder, "New File, name it "index.js"

## Write the Main Function

In the `pages/index.js` file, write the following code:

```jsx
export default () => <div>It's working!</div>
```

> `export default` means that this is the "main" function for this JavaScript file.
When another file loads `index.js`, the other file will load the above function.


## Run the Project

In your terminal, type the following command:

`yarn run dev`

This runs the "dev" script we created in [add a `dev` script](#add-a-dev-script).


## Open the Browser

Open your browser, such as "Chrome", to [http://localhost:3000](http://localhost:3000)
to see your main function in action.