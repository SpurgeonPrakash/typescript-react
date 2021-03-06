# TypeScript React

This project kicks the tires on TypeScript with React.

This was created using `npx create-react-app ts-test --typescript`.

It uses json-server as a mock API.

## Resources

I used the following resources to build this:

- [Microsoft TS Handbook](https://github.com/Microsoft/TypeScript-Handbook)
- [Compiler / TSConfig options](https://www.typescriptlang.org/docs/handbook/compiler-options.html)
- [react-typescript-samples project](https://github.com/Lemoncode/react-typescript-samples)
- [TS tips](https://medium.com/@martin_hotell/10-typescript-pro-tips-patterns-with-or-without-react-5799488d6680)
- [Interface vs Type](https://medium.com/@martin_hotell/interface-vs-type-alias-in-typescript-2-7-2a8f1777af4c)
- [Ultimate React Component Patterns](https://github.com/Hotell/blogposts/tree/master/2018-02/ultimate-react-component-patterns) and [Medium Post](https://levelup.gitconnected.com/ultimate-react-component-patterns-with-typescript-2-8-82990c516935)
- [Multiple TS Config](https://codepunk.io/multiple-tsconfig-files-for-a-single-typescript-project/)
- [Express TS example](https://github.com/dalenguyen/rest-api-node-typescript)
- [Use TS Import() to import types (the rest of the file isn't pulled into your app, so a perf win if the file with types has runtime code your app doesn't use. Note that TypeScript is smart enough to remove imports that only use types.)](https://davidea.st/articles/typescript-2-9-import-types)
- [TS Conversion Guide - Same app written in JS and TS from Microsoft](https://github.com/Microsoft/TypeScript-React-Conversion-Guide)
- [TS with Redux](https://medium.com/@rossbulat/how-to-use-typescript-with-react-and-redux-a118b1e02b76)

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Key Concepts

In TypeScript, two types are compatible if their internal structure is compatible.
`&` - Intersection operator (create a new type by intersecting one or more types or interfaces)
`Partial<Shape & Perimeter>` - Partial mapped type

### [Type vs interface](https://medium.com/@martin_hotell/interface-vs-type-alias-in-typescript-2-7-2a8f1777af4c)

1. Can't use `implements` on class with a union type
2. Can't use `extends` on interface with a union type
3. Declaration merging doesn't work with type. So use interface for public API definition when authoring a library or 3rd party ambient type definitions. Why? Interfaces can be merged (you can declare the same interface twice). Types don't support that.

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.<br>
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br>
You will also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.<br>
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.<br>
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br>
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (Webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).
