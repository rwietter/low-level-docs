# Boolean Algebra

## AND (&&)

AND is a binary operator that returns true if both operands are true, and false otherwise.

```js
true && true; // true
true && false; // false
false && true; // false
false && false; // false
```

Table of truth for AND:

| A     | B     | A && B |
| ----- | ----- | ------ |
| false | false | false  |
| false | true  | false  |
| true  | false | false  |
| true  | true  | true   |

## OR (||)

OR is a binary operator that returns true if at least one of the operands is true, and false otherwise.

```js
true || true; // true
true || false; // true
false || true; // true
false || false; // false
```

Table of truth for OR:

| A     | B     | A \|\| B |
| ----- | ----- | -------- |
| false | false | false    |
| false | true  | true     |
| true  | false | true     |
| true  | true  | true     |


## NOT (!)

NOT is a unary operator that returns true if the operand is false, and false otherwise.

```js
!true; // false
!false; // true
```

Table of truth for NOT:

| A     | !A    |
| ----- | ----- |
| false | true  |
| true  | false |

## XOR (^)

XOR is a binary operator that returns true if exactly one of the operands is true, and false otherwise.

```js
true ^ true; // false
true ^ false; // true
false ^ true; // true
false ^ false; // false
```

Table of truth for XOR:

| A     | B     | A ^ B |
| ----- | ----- | ----- |
| false | false | false |
| false | true  | true  |
| true  | false | true  |
| true  | true  | false |

## NAND

NAND is a binary operator that returns true if at least one of the operands is false, and false otherwise.

```js
!(true && true); // false
!(true && false); // true
!(false && true); // true
!(false && false); // true
```

Table of truth for NAND:

| A     | B     | !(A && B) |
| ----- | ----- | --------- |
| false | false | true      |
| false | true  | true      |
| true  | false | true      |
| true  | true  | false     |

## NOR

NOR is a binary operator that returns true if both operands are false, and false otherwise.

```js
!(true || true); // false
!(true || false); // false
!(false || true); // false
!(false || false); // true
```

Table of truth for NOR:

| A     | B     | !(A   \|\| B) |
| ----- | ----- | ------------- |
| false | false | true          |
| false | true  | false         |
| true  | false | false         |
| true  | true  | false         |

## XNOR

XNOR is a binary operator that returns true if both operands are true or both operands are false, and false otherwise.

```js
!(true ^ true); // true
!(true ^ false); // false
!(false ^ true); // false
!(false ^ false); // true
```

Table of truth for XNOR:

| A     | B     | !(A ^ B) |
| ----- | ----- | -------- |
| false | false | true     |
| false | true  | false    |
| true  | false | false    |
| true  | true  | true     |
