---
author:
- David Sanson
title: 'Phi 112: Day 5'
subtitle: Translation
date: 27 August 2020
title-slide-attributes:
    data-background-image: img/escherdogs.jpg
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


# Agenda

-   Check in
-   Overview of Unit 3
-   Breakout: Depends

-----

-   [Overview] now includes links to slides
-   Experimental "worksheets" at the top of assignments
-   Zoom XP not yet added (getting there!)
-   Retakes in full swing!
-   Unit 3 posted
-   Office Hours: TuTh noon to 1pm on Discord

-----

-   Issues, Questions, Puzzles, Uncertainties?

# Unit 3: Translation

-   Symbols to English
-   English to Symbols

## Translation: Why?

-   A chance to *think more clearly* about the logical form of English.
-   Learn to *read* our symbolic sentences as *meaningful sentences*.
-   Allows us to *apply our formal tools* to English arguments.

## Canonical Translations

  Name             Symbolic        Canonical English
  --------------- ---------- -----------------------------
  Negation            ¬▢      it is not the case that ▢
  Conjunction       (▢∧◯)           (both ▢ and ◯)
  Disjunction       (▢∨◯)           (either ▢ or ◯)
  Conditional       (▢→◯)            (if ▢ then ◯)
  Biconditional     (▢↔◯)        (▢ if and only if ◯)

## Scheme of Abbreviation{.twocolumn}

:::{.standardform  .nobullets}
| P: Putin is watching.
| Q: The Kremlin is on to you.
| R: Russia knows about your scheme.
::: 
:::{.standardform  .nobullets}

| P: Neon is a noble gas.
| Q: Neon is inert.
| R: Neon is safe to eat.
:::

# Symbols to English

## The Process

1.  Rewrite in official notation.
2.  Replace main connective with canonical English.
3.  Replace main connectives of remaining parts with canonical English.
4.  Continue until the only non-English bits are the sentence letters.
5.  Replace the sentence letters with English sentences.

## Step 1{data-transition="fade"}


1.  Rewrite in official notation.

::: {.nobullets}
-   $\mathrm{P\mathbin{\wedge} Q\mathbin{\rightarrow} R}$
:::

::: {.nobullets .incremental}
-   $\mathrm{((P\mathbin{\wedge} Q)\mathbin{\rightarrow} R)}$
:::

## Step 2{data-transition="fade"}

2.  Replace main connective with canonical English.

::: {.nobullets}
-   $\mathrm{((P\mathbin{\wedge} Q)\mathbin{\rightarrow} R)}$
:::

::: {.incremental .nobullets}
-   (If $\mathrm{(P\mathbin{\wedge} Q)}$ then $\mathrm{R}$)
:::

## Steps 3 and 4{data-transition="fade"}

3.  Replace main connectives of remaining parts
4.  Continue until the only non-English bits are the sentence letters.

::: {.nobullets}
-   (If $\mathrm{(P\mathbin{\wedge} Q)}$ then $\mathrm{R}$)
:::

::: {.incremental .nobullets}
-   (If (both $\mathrm{P}$ and $\mathrm{Q}$) then $\mathrm{R}$)
:::

## Step 5{data-transition="fade"}

5.  Replace the sentence letters with English sentences.

::: {.nobullets}
-   (If (both $\mathrm{P}$ and $\mathrm{Q}$) then $\mathrm{R}$)
:::

::: {.incremental .nobullets}
-   (If (both Putin is watching and the Kremlin is on to you) then Russia
    knows your scheme)
:::

# English to Symbols

## Canonical English

-   For a sentence in our "canonical" English, just reverse the process.
-   It is not the case that (either Putin is watching or Russia knows your
    scheme)
-   It is not the case that (either $\mathrm{P}$ or $\mathrm{R}$)
-   It is not the case that $\mathrm{(P\mathbin{\vee} R)}$
-   $\mathrm{\mathord{\neg} (P\mathbin{\vee} R)}$

## Actual English

-   English doesn't usually come in our preferred "canonical" form.
-   And that makes it is harder to translate!

## Conditionals in English

Antecedent
:   The *antecedent* is the "if-part" of a conditional.

Consequent
:   The *consequent* is the "then-part" of a conditional.

::: {.incremental}
-   If [shit happens]{.A} then [we will make do]{.B}
-   [shit happens]{.A} is the antecedent.
-   [we will make do]{.B} is the consequent.
:::

## 'If' and 'Then'

-   'if' is an antecedent marker:
    -   *If* [complete sentence]{.A} then blah blah blah
-   'then' is a consequent marker:
    -   If blah blah blah *then* [complete sentence]{.B}
-   English is lazy, and often omits 'then':
    -   If [complete sentence]{.A} [complete sentence]{.B}

## Order Issues

-   In symbols, the antecedent *always* goes *before* the arrow: [P]{.A}→Q
-   English is flexible about the order of expression of antecedent and
consequent.

::: {.incremental}
-   If [shit happens]{.A} we will make do
-   We will make do if [shit happens]{.A}
:::

## 'Only if'{data-transition="fade"}

  T                                  F                                  Sentence
  ---------------------------------- ---------------------------------- -------------------------------------------
  `<input type="checkbox">`{=html}   `<input type="checkbox">`{=html}   You can vote only if you are 18 or older.
  `<input type="checkbox">`{=html}   `<input type="checkbox">`{=html}   You can vote if you are 18 or older.
  `<input type="checkbox">`{=html}   `<input type="checkbox">`{=html}   If you are 18 or older, you can vote.
  `<input type="checkbox">`{=html}   `<input type="checkbox">`{=html}   If you can vote, you are 18 or older.

:::incremental
-   'Only if' is a *consequent marker*.
:::

## Other Antecedent Markers

-   *Stylistic variants* of 'if':
    -   'Provided that'
    -   'On the condition that'
    -   'Assuming that'
-   These are *all* antecedent markers
-   They can *all* be transformed into consequent markers by 'only'

## 'But' and 'Unless'

-   'But' means 'and'!
    -   The Bulls play basketball but they don't play it well.
    -   Both *the Bulls play basketball* and *they don't play it well.
-   'Unless' means 'or'!
    -   I don't watch the NBA unless the Bulls are playing.
    -   Either *I don't watch the NBA* or *the Bulls are playing*. 

## Stylistic Variants of 'But'

-   These *all* express (surprising) conjunctions
    -   'But'
    -   'However'
    -   'Although'
    -   'Even though'

# Breakout Groups

## Choose Your Own Adventure

-   Y'all have spread out, and you're all working on different things.
-   I have three groups planned: a Unit 1 group, a Unit 2 group, and a Unit 3
    group.
-   It is up to you which group you want to join.
-   If you regret your decision, leave the group, and I can put you into
    another group instead.

## Option 1: Unit 1

-   This is a *reading group* for people who have not yet started on Carnap,
    or are still working through Unit 1.
-   Your collective goal is to *read* and *discuss* the Unit 1 Reading,
    answering the reading questions as you go.
-   If you finish that, then your goal is to tackle the Unit 1 Exercises.
-   To join this group, rename yourself so your name starts with "1"

## Option 2: Unit 2

-   This is also a group for folks working on Unit 2, or about to tackle Unit
    2
-   Your collective goal is to *read* and
    *discuss* the Unit 2 Reading and/or work through the Unit 2 Exercises.
-   If you have already completed the exercises, but feel like you don't
    understand them, this is the group for you! Don't just "get the answers".
    Try to figure out, together, why those are the *right* answers.
-   Rename yourself so your name starts with "2"

## Option 3: Unit 3

-   If you are working on Unit 3, you are "on pace" for the course.
-   For you, I have a set of breakout room exercises in the form of a Carnap
    page that isn't an assignment, and isn't worth any points.
-   Rename yourself so your name starts with "3"

# What You Should Be Doing

-   If you haven't taken the Unit 2 Test yet, get on it!
    -   If you are further behind than that, keep moving forward!
-   Start in on Unit 3, with the plan of completing it by the end of the week.
-   Keep talking on Discord.
