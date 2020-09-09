---
author:
- David Sanson
title: 'Unit 4'
subtitle: Direct Derivations
title-slide-attributes:
    data-background-image: img/begriffschrift.png
    data-background-size: fill
    data-background-opacity: .3
theme: moon
controls: true
hashOneBasedIndex: true
hash: true
respondToHashChanges: true
history: false
center: false
...


# Direct Derivations

## Derivations

-   We call an explicit line of reasoning *from* some premises *to* a
    conclusion a *proof*.
-   In our formal system, we used *derivations* to represent *proofs*.
-   Our system will have three methods of derivation.
-   Unit 4 introduces the first method: Direct Derivation (DD)

## Basic Idea

-   To show that an argument is valid, reason step by step, following our
    rules of inference, from the premises to the conclusion.

## An Informal Example

<div class="standardform">

| [If it rains, streets get wet]{.premise .nn}
| [If streets get wet, roads are slippery]{.premise .nn}
| [It rains]{.premise .nn}
| [Roads are slippery]{.conclusion}

</div>

## An Informal Example

:::{.proof .incremental}

1. [*Roads are slippery*]{.show}
2. [If it rains, streets get wet (PR)]{.indent}
3. [If streets get wet, roads are slippery (PR)]{.indent}
4. [It rains (PR)]{.indent}
5. [Streets get wet (MP 2,4)]{.indent}
6. [*Roads are slippery* (MP 2,5)]{.indent}
7. [DD 6]{.premise}

:::

## The Same Example, Formally

:::{.standardform}

| [$R \rightarrow  W$]{.premise .nn}
| [$W \rightarrow  S$]{.premise .nn}
| [$R$]{.premise .nn}
| [$S$]{.conclusion}

:::

## The Same Example, Formally

:::{.proof .incremental}

1.  [$S$]{.show}
2.  [$R\rightarrow W$ [PR]{.just}]{.indent}
3.  [$W\rightarrow S$ [PR]{.just}]{.indent}
4.  [$R$ [PR]{.just}]{.indent}
5.  [$W$ [MP 2,4]{.just}]{.indent}
6.  [$S$ [MP 2,5]{.just}]{.indent}
7.  [:DD 6]{.premise}

:::

## Examples in Carnap

<iframe
data-src="https://carnap.io/shared/dsanson@gmail.com/unit-04-dd-examples"
width="600" height="480" frameborder="0" marginwidth="0" marginheight="0" 
scrolling="yes" style="border:3px solid #666; margin-bottom:5px; max-width:
100%;" allowfullscreen="yes"></iframe>


