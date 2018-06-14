To reproduce the bug:

```sh
npm install
npm run demo
```

The error `.../GraphQL request: Syntax Error: Unexpected Name "IBar"` will
occur. It looks like apollo-codegen chokes on the syntax to implement multiple
interfaces in the same type (see schema.graphql).