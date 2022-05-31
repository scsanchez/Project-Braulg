# Braulg - Travel social app

## Front-End Manual Installation:

- Make sure you are using node version 16+.

1. Install the packages: `$ npm install`
2. Start the webpack dev server `$ npm run start`

## Context

This project comes with a centralized general Context API. The file `./src/js/store/flux.js` has a base structure for the store.

React Context [docs](https://reactjs.org/docs/context.html)

The `Provider` is already set. You can consume from any component using the useContext hook to get the `store` and `actions` from the Context.

```jsx
import { Context } from "../store/appContext";
const MyComponentSuper = () => {
  //here you use useContext to get store and actions
  const { store, actions } = useContext(Context);
  return <div>{/* you can use your actions or store inside the html */}</div>;
};
```