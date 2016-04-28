---
layout: post
title: "floating point"
publish: true
---

### IEEE standard
(-1)^s M 2^E

s + exp + frac

exp encode E, frac encode M

single precision: 1 + 8 + 23

double precision: 1 + 11 + 52

### Different values

Normalized values

Condition: exp != 0000... , and exp != 1111..

Encode E as

E = Exp - bias

Bias = 2^k-1 - 1

M coded with implied leading 1

M = 1...

Minimum : fac = 0000... (M=1.0)

Maximum : frac = 1111... (M = 2.0-epsilon)

12345 = 1.1000000111001*2^13

s = 0
E = 13
Exp = 140
frac = 1000000111001...0

### Denormalized values

exp = 00000

E = 1-frac

### Special values
exp = 111...

exp = 111... frac = 000

exp = 111... frac != 0000...

positive

### denormalized:

bias = 3

1-bias = -2

0 000 00/01/10/11 => 1*2^(-2)×0.(0/1/2/3)

### normalized:

0 001 000 smallest normalized value 1.0 * 1.()

0 110 111

### Special values

0 111 000 inf

0 111 *** not a number



**How floating points are calculated??**


### Compare

 
