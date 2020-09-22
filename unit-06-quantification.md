---
author:
- David Sanson
title: Quantifier Terms
title-slide-attributes:
    data-background-image: img/spice.jpg 
    data-background-size: fill
    data-background-opacity: .2
theme: moon
controls: true
hashOneBasedIndex: true
hash: true
respondToHashChanges: true
history: false
center: false
...

# Quantifier Terms

## Basics

-   A quantifier term is a phrase like 'all' or 'some' or 'none', or 'all of
    us', 'some of us', 'none of us'.
-   If we know who all we are talking about, we can translate many sentences in
    English that contain quantifier terms, using conjunctions, disjunctions,
    and negations.

## Example 1

::: {.increment}
-   Suppose we are the Spice Girls: Scary, Sporty, Baby, Ginger, and Posh.
-   Then we can unpack the claim,
    -   'All of us are famous'
    -   'Scary and Sporty and Baby and Ginger and Posh are famous'
    -   $P\wedge Q\wedge R\wedge S\wedge T$
:::

## Example 2

::: {.increment}
-   'Not all of us are famous'
-   'It is not the case that (Scary and Sporty and Baby and Ginger and Posh
    are famous)'
-   $\neg(P\wedge Q\wedge R\wedge S\wedge T)$
:::

## Example 3

::: {.increment}
-   'At least one of us is famous'
-   'Scary or Sporty or Baby or Ginger or Posh is famous'
-   $P\vee Q\vee R\vee S$
:::

## Example 4

::: {.increment}
-   'Some of us are famous'
-   'At least one of us is famous'
-   'Scary or Sporty or Baby or Ginger or Posh is famous'
-   $P\vee Q\vee R\vee S$
:::

## Example 5

::: {.increment}
-   'None of us are famous'
-   'It is not the case that at least one of us is famous'
-   $\neg(P\vee Q\vee R\vee S)$
-   'All of us are not famous'
-   $\neg P\wedge \neg Q\wedge \neg R\wedge \neg S$
:::

## Limitations

-   This approach works best for *restricted* quantifier phrases (like 'all of
    us'), where the collection of individuals is small, and we *know* who all
    the individuals in the group are.
-   Symbolic sentences are long and unwieldy for large collections. Imagine
    symbolizing 'All ISU students are Redbirds' using this method.
-   It won't work at all for infinite collections: 'All even numbers are
    divisible by two'

