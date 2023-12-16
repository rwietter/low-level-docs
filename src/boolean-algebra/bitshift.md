# Bitshift

## Left Shift

The left shift operator `<<` shifts the bits of the first operand to the left by the number of bits specified by the second operand. Excess bits shifted off to the left are discarded. Zero bits are shifted in from the right.

```js
0b1010 << 1 // 0b10100 (10 << 1 = 20) -> add a zero to the right
```

## Right Shift

The right shift operator `>>` shifts the bits of the first operand to the right by the number of bits specified by the second operand. Excess bits shifted off to the right are discarded. Copies of the leftmost bit are shifted in from the left.

```js
0b1010 >> 1 // 0b101 (10 >> 1 = 5) -> remove the rightmost bit
```