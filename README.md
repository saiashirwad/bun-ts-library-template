# Texoport's Bun Library Template

* rename @texoport/template to @texoport/your-library

* package.json
```json
"exports": {
  ".": {
    "types": "./dist/index.d.ts",
    "default": "./dist/index.js"
  },
  "your-export": {
    "types": "./dist/your-export.d.ts",
    "default": "./dist/your-export.js"
  }
}

```
* build.ts
```ts
const config = {
  ...,
  entrypoints: ['./src/index.ts', './src/your-export.ts'],
}
```
