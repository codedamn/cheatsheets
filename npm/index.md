# NPM

NPM is a package manager for Node.JS (JavaScript Runtime Environment). npm is written entirely in JavaScript and was developed by Isaac Z. 

## `npm i <package-name>` (or) `npm install <package-name>`


## `npm view <package-name>`

## `npm init`

## `npm init -y`

## `npm install -g <package-name>` (or) `npm install --global <package-name>`

## `npm remove <package-name>` (or) `npm uninstall <package-name>`

## `npm root -g` 
Shows all the global modules installed on your computer

##  Dev Dependencies `npm install <package-name> --save-dev`

## Peer Dependencies 

## NODE_ENV
### Production

### dev
 
## Semantic Versioning (MAJOR.MINOR.PATCH)

1. MAJOR should be updated when you make incompatible changes.
2. MINOR should be updated version when you add functionality in a backwards compatible manner.
3. PATCH should be updated version when you make backwards compatible bug fixes.

Example : React 16.3.12

16 -> Major Version
3 -> Minor Version
12 -> Patch Version

## Symbols in Semantic Versioning

### ^
If the version is "^4.0.0"
npm tries to update the package to maximum minor and patch versions available x,y i.e. "4.x.y"

### ~
If the version is "~4.0.0"
npm tries to update the package to maximum of its available patch x i.e. "4.0.x"

## NPM Scripts


## npm run <script-name>


## NPX
npm extended

npx allows you to run local and global binaries


## changing global modules path
Sometimes you might want to change the location of the global node_modules package location because you don't want to give administrative privileges you can always change the path.

`npm config set prefix <absolute-path>`

If you don't want to mention npx while execution global script you can add your global node_modules folder to the environment variables

## Cleaning npm cache

`npm cache clean --force`