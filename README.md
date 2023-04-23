# Prettier Basic

This is a simple prettier configuration that helps match the best coding standards. 
And by the best coding standards, I of course mean my own. I am open to suggestions and pull requests.
This standard is mostly based on airbnb's standard, but with some modifications. To install

```bash
npm install --save-dev prettier prettier-basic
# or
yarn add --dev prettier prettier-basic
```

Then add the following to your `package.json`

```json
{
  "prettier": "prettier-basic"
}
```


**Or** for your `.prettierrc` file

```json
"prettier-basic"
```

**Or** to extend and change to inferior standards, you can put this in your `.prettierrc.js` file

```javascript
module.exports = {
  ...require("prettier-basic"),
  semi: false,
};
```

### Optional Configuration
I like to add an auto format script to my `package.json` as well

```json
{
  "scripts": {
    "format": "prettier --write \"**/*.{js,jsx,ts,tsx,css,scss,md}\""
  }
}
```

then it can be run with `npm run format` or `yarn format`


### Info
Refer to the [prettier options](https://prettier.io/docs/en/options.html) for more information on the options.

Refer to the [prettier configuration](https://prettier.io/docs/en/configuration.html) for more information on configuration.