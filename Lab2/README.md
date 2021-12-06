# Lab 2: Working with multiple versions of Node

## Exercise 1: Find a sample

1. Using your browser, go to http://aka.ms/spfx-webparts
1. In the **Samples by Framework**, search for **Upgrade me** and select it to open the `README.md` file associated to that sample
1. Find the link titled **Download this as a Zip file** and download the Zip file.
1. Extract the Zip file to your working folder.
1. Open a command prompt in that folder, and type `npm install`
1. If you don't run into any errors, run `gulp build`.
1. Scream in horror because of all the error messages you'll get. That's expected!

## Exercise 2: Finding what's going on
1. Go back to https://github.com/pnp/sp-dev-fx-webparts/tree/main/samples/react-upgrade-me and take a look at the compatibility section.
1. You'll need a version of Node that is compatible with SPFx 1.4.1.
1. Go to https://nodejs.org/en/download/releases/ and look for any version of Node.js that is running v8. Pick the latest version and make note of the version number.

## Exercise 3: Install Node.js v8.x.x

1. From your command prompt, type `nvm install 8.x.x` where `8.x.x` is the version number of node you found earlier.
1. Once install type `nvm use 8.x.x` where `8.x.x` is the version number of node you found earlier.

## Exercise 4: Build the web part
1. Type `npm install`
1. Type `gulp build` 
1. If you didn't get an error, you successfully were able to build an older version of SPFx!

## Exercise 4: Go back to your previous version of Node

1. From the command prompt, type `nvm list`
1. Find the latest version of Node installed (14.x.x)
1. Type `nvm use 14.x.x` where `14.x.x` is the version of Node you found in the previous step.
