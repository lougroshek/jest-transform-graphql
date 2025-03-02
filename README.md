# jest-transform-graphql

[`graphql-tag` loader for Webpack](http://dev.apollodata.com/react/webpack.html) lets you keep GraphQL queries in separate files.

This lib makes those work in Jest.

## Usage

In your package.json,

```
  "jest": {
    "transform": {
      "\\.(gql|graphql)$": "jest-transform-graphql",
      ".*": "babel-jest"
    }
  }
```

You have to include the `.*` matcher because once you define the `transform` property, it overrides that default.

For more on configuring Jest mappers, see Jest's [Webpack tutorial](https://facebook.github.io/jest/docs/tutorial-webpack.html).

## Credits

I am forking and publishing this so it can be consumed in a project I'm working on, but full credit goes to [alexcaza](https://github.com/alexcaza) and [remind101](https://github.com/remind101).
