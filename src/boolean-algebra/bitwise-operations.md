# Bitwise Operations

## AND (&)

AND is a binary operator that returns true if both operands are true, and false otherwise.

```js
0b1010 & 0b1100; // 0b1000 (10 & 12 = 8) -> A intersection B
```

Table of truth for AND:

| A   | B   | A & B |
| --- | --- | ----- |
| 0   | 0   | 0     |
| 0   | 1   | 0     |
| 1   | 0   | 0     |
| 1   | 1   | 1     |

```math
   0101    (5)
&  1010    (10)
   -----
   0000    (result of 5 & 10)
```

## OR (|)

OR is a binary operator that returns true if at least one of the operands is true, and false otherwise.

```js
0b1010 | 0b1100; // 0b1110 (10 | 12 = 14) -> A union B
```

Table of truth for OR:

| A   | B   | A \| B |
| --- | --- | ------ |
| 0   | 0   | 0      |
| 0   | 1   | 1      |
| 1   | 0   | 1      |
| 1   | 1   | 1      |


```math
   0101    (5)
|  1010    (10)
   -----
   1111    (result of 5 | 10 = 15)
```

## NOT (~)

NOT is a unary operator that returns true if the operand is false, and false otherwise.

```js
~0b1010; // 0b0101 (~10 = -11)
```

Table of truth for NOT:

| A   | ~A  |
| --- | --- |
| 0   | 1   |
| 1   | 0   |

## XOR (^)

XOR is a binary operator that returns true if exactly one of the operands is true, and false otherwise.

```js
0b1010 ^ 0b1100; // 0b0110 (10 ^ 12 = 6) -> A symmetric difference B
```

Table of truth for XOR:

| A   | B   | A ^ B |
| --- | --- | ----- |
| 0   | 0   | 0     |
| 0   | 1   | 1     |
| 1   | 0   | 1     |
| 1   | 1   | 0     |

```math
  0101    (5 in binary)
^ 1010    (10 in binary)
  ----
  1111  (binary result = 15)

because 1 ^ 0 = 1 and 0 ^ 1 = 1
```

## Other operations

```js
let A = 0b1010; // decimal: 10
let B = 0b1100; // decimal: 12
```

### Union (A ∪ B) - elements in A or B

```js
let union = A | B; // 0b1110, decimal: 14

    0b1010
  | 0b1100
    ------
    0b1110
```

### Intersection (A ∩ B)

```js
let intersection = A & B; // 0b1000, decimal: 8
    
   0b1010
 & 0b1100
   ------
   0b1000
```

### Difference (A \ B) - elements in A that are not in B

```js
let difference = A & ~B; // 0b0010, decimal: 2

  0b1010
\ 0b1100
  ------
  0b0010
```

## Types and tips

### Swap values of two variables

```rust
fn main() {
  let mut a = 5;
  let mut b = 10;
  println!("a = {}, b = {}", a, b);
  a ^= b;
  b ^= a;
  a ^= b; // a = 10, b = 5
  println!("a = {}, b = {}", a, b);
}