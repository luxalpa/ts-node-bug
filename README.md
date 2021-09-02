# ts-node-bug

This showcases a bug when using ts-node with Yarn's pnp.

Install yarn on version 1.22 or above, `yarn` this project and run `yarn ts-node index.ts`. There will be an error:
```
error TS2307: Cannot find module 'path' or its corresponding type declarations.
```

This error does not appear when deleting the tsconfig.json or when disabling pnp (for example by switching `nodeLinker` to `node-modules`).
