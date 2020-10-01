---
author:
- David Sanson
title: Truth Tables
title-slide-attributes:
    data-background-image: img/canthandletruth.jpeg
    data-background-size: fill
    data-background-opacity: .2
theme: moon
controls: true
hashOneBasedIndex: true
hash: true
respondToHashChanges: true
history: false
center: false
css: 
  -  'https://www.davidsanson.com/css/carnap.css'
  -  'https://carnap.io/static/css/exercises.css'
js:
  - 'https://carnap.io/static/ghcjs/rts.js'
  - 'https://carnap.io/static/ghcjs/allactions/lib.js'
  - 'https://carnap.io/static/ghcjs/allactions/out.js'
...

# Characteristic Truth Tables

-   Each connective expresses a truth-function
-   We can represent the truth-function expressed by a connective by giving
    its characteristic truth table
-   You can think of the truth-table as displaying the *meaning* of a word
    like 'and' or 'if'

## Negation

<div class="itt">

   $▢$   $\neg ▢$
  ----- ----------
    T       F
    F       T

</div>

-   The truth value of negation is the opposite of the truth value of the
    negated sentence

## Conjunction

<div class="itt" rows=2>

   $▢$   $◯$   $▢\wedge ◯$
  ----- ----- ---------------
    T     T          T
    T     F          F
    F     T          F
    F     F          F

</div>

-   A conjunction is only true when both of its conjuncts are true

## Disjunction

<div class="itt" rows=2>

   $▢$   $◯$   $▢\vee ◯$
  ----- ----- -----------
    T     T        T
    T     F        T
    F     T        T
    F     F        F

</div>

-   Our disjunction is *inclusive*

## The Biconditional 

<div class="itt" rows=2>

   $▢$   $◯$   $▢\leftrightarrow ◯$
  ----- ----- ----------------------
    T     T             T
    T     F             F
    F     T             F
    F     F             T

</div>

-   The biconditional expresses *agreement*: it is true when its two
    components have the same truth value

## The Conditional

<div class="itt" rows=2>

   $▢$   $◯$   $▢\rightarrow ◯$  
  ----- ----- ------------------ 
    T     T           T          
    T     F           F          
    F     T           T          
    F     F           T          

</div>

-   The conditional is only false when it *has to be*---when it takes us from
    T to F. Otherwise, it gets to be true.

# Calculating Truth

-   Given the characteristic truth tables (and our knowledge of the syntax of
    our language) we can calculate the truth value of a complex sentence,
    given an assignment of truth values to its component sentence letters.

## Some Examples

-  [Example 1](https://carnap.io/shared/dsanson@gmail.com/tt-examples#exercise-Ex1)
-  [Example 2](https://carnap.io/shared/dsanson@gmail.com/tt-examples#exercise-Ex2)

# Calculating Truth Tables

-   A truth table lists *all possible assignments* of truth values to the
    component sentence letters
-   So it has more than one row: a row for each possible assignment

## Some Examples

-  [Example 3](https://carnap.io/shared/dsanson@gmail.com/tt-examples#exercise-Ex3)
-  [Example 4](https://carnap.io/shared/dsanson@gmail.com/tt-examples#exercise-Ex4)

# Properties of Sentences

-   We can use the truth table of a sentence to determine where it is:
-   a *logical truth* = true on every row
-   a *logical falsehood* = false on every row
-   *logically contingent* = true on some, false on some

## Some Examples

-  [Example 5](https://carnap.io/shared/dsanson@gmail.com/tt-examples#exercise-Ex5)
-  [Example 6](https://carnap.io/shared/dsanson@gmail.com/tt-examples#exercise-Ex6)
-  [Example 4](https://carnap.io/shared/dsanson@gmail.com/tt-examples#exercise-Ex4)

# Logical Equivalence

-   We can construct a truth table for more than one sentence, and use that
    table to determine whether or not two sentences are:
-   *logically equivalent* = always have the same truth values as each other

## Some Examples

-  [Example 7](https://carnap.io/shared/dsanson@gmail.com/tt-examples#exercise-Ex7)
-  [Example 8](https://carnap.io/shared/dsanson@gmail.com/tt-examples#exercise-Ex8)

# Validity

-   We can use a truth table to determine whether or not an argument is valid:
-   *truth-functionally valid* = no row with all true premises and false
    conclusion
-   *not truth-functionally valid* = at least one row with all true premises
    and false conclusion

## Examples

-  [Example 9](https://carnap.io/shared/dsanson@gmail.com/tt-examples#exercise-Ex9)
-  [Example 10](https://carnap.io/shared/dsanson@gmail.com/tt-examples#exercise-Ex10)
-  [Example 11](https://carnap.io/shared/dsanson@gmail.com/tt-examples#exercise-Ex11)

