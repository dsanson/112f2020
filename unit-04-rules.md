---
author:
- David Sanson
title: 'Unit 4'
subtitle: Inference Rules
title-slide-attributes:
    data-background-image: img/rules.webp
    data-background-size: fill
    data-background-opacity: .5
theme: moon
controls: true
hashOneBasedIndex: true
hash: true
respondToHashChanges: true
history: false
center: false
...


# Outline

-   Arguments, Proofs, and Derivations
-   Inference Rules
    -   DNI, DNE, MP, MT
-   Examples

# Arguments, Proofs, and Derivations

## Arguments

-   The premises of an argument represent what we reason *from*
-   The conclusion of an argument represents what we reason *to*.
-   But what about the *reasoning* itself?

## Proofs and Derivations

-   We call an explicit line of reasoning *from* some premises *to* a
    conclusion a *proof*.
-   In our formal system, we used *derivations* to represent *proofs*.

# Direct Derivations

## Why "Direct"?

-   Start from the premises.
-   Reason step by step until you reach the conclusion.
-   In contrast to two other forms of derivation that we introduce
    in the next unit.

## Steps and Inference Rules

-   The point of a derivation is to show that the argument is valid.
-   Each step in the derivation is a mini-argument or inference.
-   So each step has to be valid.
-   So we require each step to be an instance of an 
    inference rule, where inference rules are obviously valid patterns of arguments.

# Inference Rules

-   We introduce four inference rules.
-   Two that just involve negation
-   One that just involves conditionals
-   One that involves both
-   (We put aside the other connectives for now)

# Negations

-   Every sentence is *logically equivalent* to its double negation.
-   'I care' is *logically equivalent* to 'I don't not care'
-   $P$ is *logically equivalent* to $\neg \neg P$

## Logical Equivalence

-   Two sentences are *logically equivalent* iff it is not possible for one to
    be true but the other false. 
-   'The earth is round' and 'Some cheese stinks':
    -   Both both true, but not logically equivalent
-   'The earth is round' and 'The earth is not not round':
    -   Logically equivalent.

## Dangerous Habits from Algebra

-   $P$ and $\neg \neg P$ are different sentences. The first is atomic. The
    second is a negation.
-   Some of you will be tempted to erase this difference, by erasing the
    $\neg \neg$ from the second sentence, insisting that the two negations
    "cancel each other out".
-   But we don't want to erase the difference. We want to *see* the
    difference, and recognize that two *distinct* sentences can be \*logically
    equivalent.*

## Double Negation Introduction

-   Since $P$ and $\neg \neg P$ are logically equivalent, this argument is
    formally valid: $P ∴ \neg \neg P$
-   So this our first inference rule, *Double Negation Introduction (DNI)*:

<div class=standardform>

| [▢]{.premise .nn}
| [$\neg \neg ▢$]{.conclusion}

</div>

## Double Negation Elimination

-   Since $P$ and $\neg \neg P$ are logically equivalent, this argument is
    also formally valid: $\neg\neg P ∴ P$
-   So this our second inference rule, *Double Negation Elimination (DNE)*:

<div class=standardform>

| [$\neg \neg ▢$]{.premise .nn}
| [$▢$]{.conclusion}

</div>

# Modus Ponens

## Modus Ponens (MP)

-   We have two inference rules that involve the conditional
-   Modus Ponens (MP) ("the way of putting")
-   Modus Tollens (MT) ("the way of taking")
-   Let's start with MP

## Modus Ponens (MP)

-   Suppose you have a friend, Barney, who always smiles when he is happy:
    -   If Barney is happy, then Barney smiles.
-   Suppose that Barney is happy. 
-   It follows that Barney smiles.
-   This is Modus Ponens

## Modus Ponens (MP){data-transition="fade"}

<div class=standardform>

| [If [Barney is happy]{.A}, then [Barney smiles]{.B}]{.premise .nn}
| [[Barney is happy]{.A}]{.premise .nn}
| [[Barney smiles]{.B}]{.conclusion}

</div>

## Modus Ponens (MP){data-transition="fade"}

<div class=standardform>

| [If []{.A}, then []{.B}]{.premise .nn}
| [[]{.A}]{.premise .nn}
| [[]{.B}]{.conclusion}

</div>

## Modus Ponens (MP){data-transition="fade"}

<div class=standardform>

| [[]{.A} → []{.B}]{.premise .nn}
| [[]{.A}]{.premise .nn}
| [[]{.B}]{.conclusion}

</div>

## Modus Ponens (MP){data-transition="fade"}

<div class=standardform>

| [▢ → ◯]{.premise .nn}
| [▢]{.premise .nn}
| [◯]{.conclusion}

</div>

## Modus Ponens (MP){data-transition="fade"}

<div class="rightbox">
<div class="standardform"> 

| [▢  →  ◯]{.premise .nn}
| [◯]{.premise .nn}
| [▢]{.conclusion}

</div>
</div>
<div class="leftbox"> 
<div class="standardform"> 

| [▢ → ◯]{.premise .nn}
| [▢]{.premise .nn}
| [◯]{.conclusion}

</div>
</div>

## Modus Ponens (MP){data-transition="fade"}

<div class="rightbox">
<div class="standardform xedout"> 
| [▢  →  ◯]{.premise .nn}
| [◯]{.premise .nn}
| [▢]{.conclusion}
</div>
</div>
<div class="leftbox"> 
<div class="standardform greencheck"> 
| [▢ → ◯]{.premise .nn}
| [▢]{.premise .nn}
| [◯]{.conclusion}
</div>
</div>

## Affirming the Consequent{data-transition="fade"}

<div class="standardform xedout"> 
| [▢  →  ◯]{.premise .nn}
| [◯]{.premise .nn}
| [▢]{.conclusion}
</div>


## Affirming the Consequent{data-transition="fade"}

<div class="standardform"> 
| [▢  →  ◯]{.premise .nn}
| [◯]{.premise .nn}
| [▢]{.conclusion}
</div>

## Affirming the Consequent{data-transition="fade"}

<div class=standardform>

| [If []{.A}, then []{.B}]{.premise .nn}
| [[]{.B}]{.premise .nn}
| [[]{.A}]{.conclusion}

</div>

## Affirming the Consequent{data-transition="fade"}

<div class=standardform>

| [If [Barney is happy]{.A}, then [Barney smiles]{.B}]{.premise .nn}
| [[Barney smiles]{.B}]{.premise .nn}
| [[Barney is happy]{.A}]{.conclusion}

</div>

## Affirming the Consequent{data-transition="fade"}

<div class="standardform xedout">

| [If [Barney is happy]{.A}, then [Barney smiles]{.B}]{.premise .nn}
| [[Barney smiles]{.B}]{.premise .nn}
| [[Barney is happy]{.A}]{.conclusion}

</div>

# Modus Tollens

## Modus Tollens (MT)

-   Remember, Barney always smiles when he is happy, so:
    -   If Barney is happy, then Barney smiles.
-   Suppose Barney is not smiling.
-   Then it follows that he isn't happy.
-   This is Modus Tollens.

## Modus Tollens (MT){data-transition="fade"}

<div class=standardform>

| [If [Barney is happy]{.A}, then [Barney smiles]{.B}]{.premise .nn}
| [It is not the case that [Barney smiles]{.B}]{.premise .nn}
| [It is not the case that [Barney is happy]{.A}]{.conclusion}

</div>

## Modus Tollens (MT){data-transition="fade"}

<div class=standardform>

| [If []{.A}, then []{.B}]{.premise .nn}
| [$\neg$[]{.B}]{.premise .nn}
| [$\neg$[]{.A}]{.conclusion}

</div>

## Modus Tollens (MT){data-transition="fade"}

<div class=standardform>

| [[]{.A} → []{.B}]{.premise .nn}
| [$\neg$[]{.B}]{.premise .nn}
| [$\neg$[]{.A}]{.conclusion}

</div>

## Modus Tollens (MT){data-transition="fade"}

<div class=standardform>

| [▢ → ◯]{.premise .nn}
| [¬◯]{.premise .nn}
| [¬▢]{.conclusion}

</div>

## Modus Tollens (MT){data-transition="fade"}

<div class="rightbox">
<div class="standardform"> 

| [▢ → ◯]{.premise .nn}
| [¬▢]{.premise .nn}
| [¬◯]{.conclusion}

</div>
</div>
<div class="leftbox"> 
<div class="standardform"> 

| [▢ → ◯]{.premise .nn}
| [¬◯]{.premise .nn}
| [¬▢]{.conclusion}

</div>
</div>

## Modus Tollens (MT){data-transition="fade"}

<div class="rightbox">
<div class="standardform xedout"> 

| [▢ → ◯]{.premise .nn}
| [¬▢]{.premise .nn}
| [¬◯]{.conclusion}

</div>
</div>
<div class="leftbox"> 
<div class="standardform"> 

| [▢ → ◯]{.premise .nn}
| [¬◯]{.premise .nn}
| [¬▢]{.conclusion}

</div>
</div>

## Denying the Antecedent{data-transition="fade"}

<div class="standardform xedout"> 
| [▢ → ◯]{.premise .nn}
| [¬▢]{.premise .nn}
| [¬◯]{.conclusion}
</div>

## Denying the Antecedent{data-transition="fade"}

<div class="standardform"> 
| [▢ → ◯]{.premise .nn}
| [¬▢]{.premise .nn}
| [¬◯]{.conclusion}
</div>

## Denying the Antecedent{data-transition="fade"}

<div class=standardform>

| [If []{.A}, then []{.B}]{.premise .nn}
| [$\neg$[]{.A}]{.premise .nn}
| [$\neg$[]{.B}]{.conclusion}

</div>

## Denying the Antecedent{data-transition="fade"}

<div class=standardform>

| [If [Barney is happy]{.A}, then [Barney smiles]{.B}]{.premise .nn}
| [$\neg$[Barney is happy]{.A}]{.premise .nn}
| [$\neg$[Barney smiles]{.B}]{.conclusion}

</div>

## Denying the Antecedent

<div class="standardform xedout">

| [If [Barney is happy]{.A}, then [Barney smiles]{.B}]{.premise .nn}
| [$\neg$[Barney is happy]{.A}]{.premise .nn}
| [$\neg$[Barney smiles]{.B}]{.conclusion}

</div>

## Modus Tollens (MT){data-transition="fade"}

<div class="rightbox">
<div class="standardform"> 

| [▢ → ¬◯]{.premise .nn}
| [◯]{.premise .nn}
| [¬▢]{.conclusion}

</div>
</div>
<div class="leftbox"> 
<div class="standardform"> 

| [▢ → ◯]{.premise .nn}
| [¬◯]{.premise .nn}
| [¬▢]{.conclusion}

</div>

## Modus Tollens (MT){data-transition="fade"}

<div class="rightbox">
<div class="standardform xedout"> 

| [▢ → ¬◯]{.premise .nn}
| [◯]{.premise .nn}
| [¬▢]{.conclusion}

</div>
</div>
<div class="leftbox"> 
<div class="standardform"> 

| [▢ → ◯]{.premise .nn}
| [¬◯]{.premise .nn}
| [¬▢]{.conclusion}

</div>
</div>

## Modus Tollens (MT){data-transition="fade"}

-   One premise needs to be the *negation of the consequent* of the other:

<div class="standardform"> 

| [▢ → *◯*]{.premise .nn}
| [¬*◯*]{.premise .nn}
| [¬▢]{.conclusion}

</div>

## Modus Tollens (MT){data-transition="fade"}

-   Here the consequent is the negation of the premise:

<div class="standardform"> 

| [▢ → ¬*◯*]{.premise .nn}
| [*◯*]{.premise .nn}
| [¬▢]{.conclusion}

</div>

That's not the same thing. That's not MT.

# Examples

## Example 1

<div class="standardform">

| [$P\rightarrow Q$]{.premise .nn}
| [$\neg \neg (P\rightarrow Q)$]{.conclusion}

</div>

::: {.incremental}
-   This is an example of DNI
:::

## Example 2

<div class="standardform">

| [$\neg \neg (P\rightarrow Q)$]{.premise .nn}
| [$P\rightarrow Q$]{.conclusion}

</div>

::: {.incremental}
-   This is an example of DNE
:::

## Example 3 {#example-3 data-transition="fade"}

<div class="standardform">

| [$\neg \neg P\rightarrow Q$]{.premise .nn}
| [$P\rightarrow Q$]{.conclusion}

</div>

::: {.incremental}
-   This is *not* an example of DNE
:::

## Example 3 {#example-3-1 data-transition="fade"}

<div class="standardform">

| [$(\neg \neg P\rightarrow Q)$]{.premise .nn}
| [$P\rightarrow Q$]{.conclusion}

</div>

-   This is *not* an example of DNE

## Example 4

<div class="standardform">

| [$R\rightarrow P$]{.premise .nn}
| [$R$]{.premise .nn}
| [$P$]{.conclusion}

</div>

::: {.incremental}
-   This is an example of MP
:::

## Example 5

<div class="standardform">

| [$R\rightarrow P$]{.premise .nn}
| [$P$]{.premise .nn}
| [$R$]{.conclusion}

</div>

::: {.incremental}
-   This is *not* an example of MP or MT
:::

## Example 6

<div class="standardform">

| [$(R\rightarrow P)\rightarrow (Q\rightarrow S)$]{.premise .nn}
| [$R\rightarrow P$]{.premise .nn}
| [$Q\rightarrow S$]{.conclusion}

</div>

::: {.incremental}
-   This is an example of MP
:::

## Example 7

<div class="standardform">

| [$\neg R\rightarrow \neg S$]{.premise .nn}
| [$\neg R$]{.premise .nn}
| [$\neg S$]{.conclusion}

</div>

::: {.incremental}
-   This is an example of MP
:::

## Example 8

<div class="standardform">

| [$\neg R\rightarrow \neg S$]{.premise .nn}
| [$\neg S$]{.premise .nn}
| [$\neg R$]{.conclusion}

</div>

::: {.incremental}
-   This is not an example of MP or MT
:::

## Example 9

<div class="standardform">

| [$\neg R\rightarrow \neg S$]{.premise .nn}
| [$\neg \neg S$]{.premise .nn}
| [$\neg \neg R$]{.conclusion}

</div>

::: {.incremental}
-   This is an example of MT
:::

## Example 10

<div class="standardform">

| [$\neg R\rightarrow \neg S$]{.premise .nn}
| [$S$]{.premise .nn}
| [$R$]{.conclusion}

</div>

::: {.incremental}
-   This is not an example of MP or MT
:::

## Example 11

<div class="standardform">

| [$(\neg R\rightarrow \neg S)\rightarrow \neg \neg (S\rightarrow P)$]{.premise
  .nn}
| [$\neg \neg ((\neg R\rightarrow \neg S)\rightarrow \neg \neg (S\rightarrow P))$]{.conclusion}

</div>

::: {.incremental}
-   This is an example of DNI
:::

## Example 11

<div class="standardform">

| [$(\neg R\rightarrow \neg S)\rightarrow \neg \neg (S\rightarrow P)$]{.premise
  .nn}
| [$(\neg R\rightarrow \neg S)\rightarrow (S\rightarrow P)$]{.conclusion}

</div>

::: {.incremental}
-   This is not an example of DNE
:::

# Summary

-   We have four inference rules:
    -   DNE, DNI, MP, MT
-   In the next lecture, we will look at how to use them to construct
    derivations.
