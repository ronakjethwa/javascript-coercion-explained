# JavaScript Coercion

JavaScript Coercion is confusing, complex and often gets asked in interviews. This article goes in-depth on how type coercion works in JavaScript. These rules, tricks and tips will help you ace that next interview.

There are two types of coercion in JavaScript. `Implicit` and `Explicit`. When a developer expresses the intention to convert between types by writing the appropriate code, like Number(value), it’s called explicit type coercion (or type casting). Everyone knows what these are. The complexity comes while doing implicit coercion, which happens when you apply operators to values of different types.

These document goes in-depth on the `Implicit` coercion.

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
Arithmetic addition operator, triggers numeric conversion to string if one of them is string.
Arithmetic addition operator, triggers string conversion to numeric if both of them are string numeric.
```javascript
12 + "" --> "12"
"15" + 2 --> 152
"4" - "3" --> 1
undefined + 3 -- > NaN
"Hello" + null --> "Hellonull"
null + 5 --> 5
true + 10 --> 11
"number" + 1 + 2 --> "number12"
```




