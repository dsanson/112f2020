---
author:
- David Sanson
title: Conditional and Indirect Derivations
title-slide-attributes:
    data-background-image: https://imgs.xkcd.com/comics/hypotheticals.png
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

# Outline

-   Conditional Derivations
-   Indirect Derivations
-   Subderivations
-   Theorems

# Conditional Derivations

## Basics

-   A conditional derivation is a formal representation of a conditional
    proof.
-   Conditional proof is a familiar pattern of hypothetical reasoning.
-   The basic idea: to prove an *if...then...*, assume that the
    *if...* is true, and show that, from this assumption, the *then...* follows.

# Conditional Proofs

## First Example

*Show*
:   If [you live in Toronto]{.A}, then [you live in Canada]{.B}.

*Proof*
:   Suppose [you live in Toronto]{.A}. Toronto is a city in Canada, so anyone
who lives in Toronto lives in Canada. So, given our assumption, it follows
that [you live in Canada]{.B}.

## Second Example

*Show*
:    If [I have hands]{.A}, then [the external world exists]{.B}.

*Proof*
:    Suppose [I have hands]{.A}. Hands are objects in the external
world. So, given our assumption, it follows that [the external world
exists]{.B}.

## Third Example

*Show*
:    If [the King fails to execute Naṣr al-Dīn]{.A}, then [the King should
be executed]{.B}.

*Proof*
:    Suppose [the King fails to execute Naṣr al-Dīn]{.A}. Then Naṣr al-Dīn's
claim, "I will be executed", was a lie. So the King was lying when he said
that all liars will be executed. So, by his own decree, [the King should be
executed]{.B}.

## Fourth Example

*Show*
:    If [God exists]{.A}, then [free will is an illusion]{.A}.

*Proof*
:    Suppose God exists. By definition, God is all-knowing, and cannot be
mistaken. So, for anything I do, she already knows that I will do it before I
do it. But that means I can't do otherwise: If I could, then God could be
mistaken. But she can't be mistaken. So I can't. And if I can't do otherwise,
then free will is an illusion.

# Conditional Derivations

## The Basic Pattern

:::{.proof .incremental}

1.  [▢→◯]{.show}
2.   [▢       [AS]{.just}]{.indent}
3.   [⋮]{.indent}
4.   [⋮]{.indent}
5.   [◯]{.indent}
6. [:CD 5]{.premise}

:::

## An Example

$P\rightarrow Q, Q\rightarrow R \vdash P\rightarrow R$

:::{.proof .incremental}

1.  [P→R]{.show}
2.   [P       [AS]{.just}]{.indent}
3.   [P→Q     [PR]{.just}]{.indent}
4.   [Q       [MP 2,3]{.just}]{.indent}
5.   [Q→R     [PR]{.just}]{.indent}
6.   [R       [MP 4,5]{.just}]{.indent}
7. [:CD 6]{.premise}

:::

## Some Examples in Carnap

:::{.carnap-embed .stretch}

<iframe
data-src="https://carnap.io/shared/dsanson@gmail.com/unit-05-examples"
width="1000" height="400" frameborder="0" marginwidth="0" marginheight="0" 
scrolling="yes" allowfullscreen="yes"></iframe>

:::

# Indirect Derivations

## Basics

-   Indirect Derivation represents an indirect proof, also known as a proof by
    *reductio ad absurdum*.
-   The basic idea: to prove that something is false, show that, if it were
    true, a contradiction would follow.

# Indirect Proofs

## First Example

*Show*
:    It is not the case that [God exists]{.A}.

*Proof*
:    Suppose [God exists]{.A}. By definition, she is all-good,
all-powerful, and all-knowing. So she won't allow any evils to occur. But
evils do occur. So the assumption that God exists leads to a
contradiction. So God doesn't exist.

## First Example {data-transition="fade"}
*Show*
:    It is not the case that [God exists]{.A}.

*Proof*

:   | Suppose [God exists]{.A}.
    | ⋮
    | [There is evil]{.B}.
    | Not [there is evil]{.B}.

## Second Example 

*Show*
:   Not all sentences are false.

*Proof*
:   Assume that all sentences are false. But then the sentence 'All
sentences are false' is true, which contradicts our assumption.

## Second Example {data-transition="fade"} 

*Show*
:   Not [all sentences are false]{.A}.

*Proof*

:   | Assume that [all sentences are false]{.A}.
    | ⋮
    | ['All sentences are false' is true]{.B}.
    | Not ['All sentences are false' is true]{.B}.

## Third Example 

*Show*
:   There is no greatest natural number.

*Proof*
:   Assume there is a greatest natural number, $n$. Then $n+1$ is also a
    natural number, and is greater than $n$. But that contradicts our
    assumption that $n$ is the greatest natural number.

## Third Example {data-transition="fade"}

*Show*
:   Not [there is a greatest natural number]{.A}.

*Proof*

:   | Assume [there is a greatest natural number]{.A}, $n$.
    | ⋮
    | [$n+1$ is greater than $n$]{.B}
    | Not [$n+1$ is greater than $n$]{.B}

# Indirect Derivations

## The Basic Pattern

:::{.proof .incremental}

1.  [¬▢]{.show}
2.   [▢       [AS]{.just}]{.indent}
3.   [⋮]{.indent}
4.   [⋮]{.indent}
5.   [◯]{.indent}
6.   [¬◯]{.indent}
7. [:CD 5,6]{.premise}

:::

## An Example

$P\rightarrow Q, Q\rightarrow \neg P \vdash \neg P$

:::{.proof .incremental}

1.  [¬P]{.show}
2.   [P       [AS]{.just}]{.indent}
3.   [P→Q     [PR]{.just}]{.indent}
4.   [Q       [MP 2,3]{.just}]{.indent}
5.   [Q→¬P     [PR]{.just}]{.indent}
6.   [¬P       [MP 4,5]{.just}]{.indent}
7. [:ID 2,6]{.premise}

:::

## Some Examples in Carnap

:::{.carnap-embed .stretch}

<iframe
data-src="https://carnap.io/shared/dsanson@gmail.com/unit-05-examples#indirect-derivations"
width="1000" height="400" frameborder="0" marginwidth="0" marginheight="0" 
scrolling="yes" allowfullscreen="yes"></iframe>

:::

# Subderivations

## Basics

-   A subderivation is a derivation *inside* another derivation
-   To start a subderivation, enter a second show line.

## Examples in Carnap

:::{.carnap-embed .stretch}

<iframe
data-src="https://carnap.io/shared/dsanson@gmail.com/unit-05-examples#subderivations"
width="1000" height="400" frameborder="0" marginwidth="0" marginheight="0" 
scrolling="yes" allowfullscreen="yes"></iframe>

:::


# Theorems

## Basics

-   A theorem is a sentence that can be derived from no premises.
-   All theorems are *logical truths*.
-   Examples: $P\rightarrow P$, $P\rightarrow \neg \neg P$.

## Examples in Carnap

:::{.carnap-embed .stretch}

<iframe
data-src="https://carnap.io/shared/dsanson@gmail.com/unit-05-examples#theorems"
width="1000" height="400" frameborder="0" marginwidth="0" marginheight="0" 
scrolling="yes" allowfullscreen="yes"></iframe>

:::
