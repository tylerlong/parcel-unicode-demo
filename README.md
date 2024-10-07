# Parcel Unicode Demo

As I tested, parcel does not support unicode characters in variable names. This is a demo to show that.

Ref: https://github.com/parcel-bundler/parcel/issues/9607

```ts
const µ = 'a';
console.log(µ);
```

Will be compiled to:

```js
var \xb5 = "a";
console.log(\xb5);
```
