# JavaScript Coercion

JavaScript Coercion is confusing, complex and often gets asked in interviews. This article goes in-depth on how type coercion works in JavaScript. These rules, tricks and tips will help you ace that next interview.

There are two types of coercion in JavaScript. `Implicit` and `Explicit`. When a developer expresses the intention to convert between types by writing the appropriate code, like Number(value), it’s called explicit type coercion (or type casting). Everyone knows what these are. The complexity comes while doing implicit coercion, which happens when you apply operators to values of different types.

These document goes in-depth on the `implicit` coercion.

## Rules Of Implicit Coercion

### Booleans
Binary + operator triggers numeric conversion for true and false
```javascript
true + false --> 1
true + true --> 2
false + false --> 0
```

### `/` Operations
Arithmetic division operator / triggers numeric conversion for string
```javascript
12 / '6' --> 2
'12' / '6' --> 2 
```

### `+` Operations
  



