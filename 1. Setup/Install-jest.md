From [https://jestjs.io/docs/getting-started](https://jestjs.io/docs/getting-started)

# Using Jest with React:
You will be using the following tools:
1. Jest (testing language)
2. React-Testing-Library (testing library specific to React)
3. JSDOM (in order to "render" components, you must use)
4. Babel (in order to "render" components, you muse use)

# Set up Jest
1. Make sure you have a React program already initialized with either Parcel or Babel
1. Install jest globally (recommended) using `npm install jest --global`
1. Create a basic configuration file using `jest --init`
  * You want to use Jest when you run `npm run test`
  * You want to use jsdom as your testing interface
  * You want to use Babel
  * You *probably* want to clear all mocks after each test (at least, you will want to for this tutorial)
4. Create a `.babelrc` file inside the root project directory. Inside of it, include the following:
```javascript
// .babelrc
{
  "presets": [
    "@babel/preset-env",
    "@babel/preset-react"
  ]
}
```