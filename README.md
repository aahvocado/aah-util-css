# aah-util-css
This is a work in progress, and is still incomplete. This utility css uses [less](http://lesscss.org) for the framework.

This utility now supports `sass` and needs updated documentation.

## usage
`npm i aah-util-css`

## customizing
You can use it as is, or if you want to customize the colors you'll to have `less cli` installed.

Create a `definitions.less` file and customize the variables like here https://github.com/aahvocado/aah-util-css/blob/master/definitions.less

Then create an app level less file. Example `app.less`:
```
@import 'definitions.less'; // create this
@import 'aah-util-css/all-util-styles.less'; // from an imported package
```

Then you should be able to compile the styles like so
`lessc src/styles/app.less src/build/app.css`
