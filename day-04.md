---
author:
- David Sanson
title: 'Phi 112: Day 4'
subtitle: Sentential Logic
date: 27 August 2020
title-slide-attributes:
    data-background-image: img/syntax.jpg
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

-   Course/Tech support?
-   Sentential Logic Symbols
-   Sentential Logic Syntax
-   Informal Notation

-----

-   Zoom XP not yet added (getting there!)
-   Discord: ongoing bot problems (@ me if your stats need adjusting)
-   Retakes in full swing!
-   Unit 3 not yet posted.
-   Office Hours?

# Sentential Logic: Symbols
    
## Symbols

  Name             Symbol        English Meaning
  --------------- -------- ---------------------------
  Conjunction        ∧                'and'
  Disjunction        ∨                'or'
  Conditional        →           'if...then ...'
  Biconditional      ↔          'if and only if'
  Negation           ¬      'it is not the case that'

## Simple Sentences

  ----- ---------------------------
     ¬P It is not the case that P
    P→Q If P, then Q.
    P∧Q Both P and Q.
    P∨Q Either P or Q.
  ----- ---------------------------

## English Examples

  ----------------- -----------------------------------------------------------------
           ¬[P]{.P} It is not the case that [the pie is ready]{.P}.
    [P]{.P}→[Q]{.Q} If [the pie is ready]{.P}, then [we eat it]{.Q}.
    [P]{.P}∧[Q]{.Q} Both [the pie is ready]{.P} and [we eat it]{.Q}.
    [P]{.P}∨[Q]{.Q} Either [the pie is ready]{.P} or [we eat it]{.Q}.
  ----------------- -----------------------------------------------------------------

# Sentential Logic: Syntax

## "Syntax"

-   'Syntax' is another word for grammar.
-   It is a set of rules that tell you when a combination of words makes a
    grammatically well-formed sentence.
-   'Dog the of bark': not a well-formed sentence.
-   'Dogs bark': a well-formed sentence.

## Syntax for Natural Languages

-   The syntax of a *Natural* Language like English is super complicated.
-   (and super neat: there is an entire branch of Linguistics devoted to the
    study of syntax in natural languages.)
-   It's amazing that we all recognize grammatical errors, given how
    complicated the rules are, and we can't actually *say* what those rules
    are.

## Syntax for Sentential Logic

1.  Every sentence letter 'P', 'Q', 'R', ...,
    'Z' is a sentence. And so are the sentence letters with
    subscripts.
2.  If '▢' is a sentence, then '¬▢ ' is too.
3.  If '▢' and '◯' are both sentences, then:
    a.  '(▢ ∧ ◯ )' is also a sentence, and
    b.  '(▢ ∨ ◯ )' is also a sentence, and
    c.  '(▢ → ◯ )' is also a sentence, and
    d.  '(▢ ↔ ◯ )' is also a sentence.

## Examples of Sentences

(P → Q)

<div class="incremental">

-   'P' and 'Q' are sentences, by rule 1.
-   So '(P → Q)' is a sentence, by rule 3c.

</div>

## Examples of Sentences

¬(P → Q)

<div class="incremental">

-   We just saw that '(P → Q)' is a sentence.
-   So '¬(P→Q)' is a sentence, by rule 2.

</div>

## Examples of Sentences

¬¬¬¬¬¬¬¬¬Z 

<div class="incremental">

-   'Z' is a sentence by rule 1.
-   So '¬Z' is a sentence by rule 2.
-   So '¬¬Z' is a sentence by rule 2.
-   So '¬¬¬Z' is...

</div>

## Examples of Sentences

((P ∧ Q) ∨ (Q → R))

<div class="incremental">

-   '(P ∧ Q)' is a sentence, by rule 1 and then rule 3a.
-   '(Q → R)' is, by rule 1 and then rule 3c.
-   So '((P ∧ Q) ∨ (Q → R))', by rule 3b.

</div>

## Examples of Sentences

(((P ∧ Q) ∨ (Q → R))↔ ¬¬¬¬¬¬¬¬¬Z)

<div class="incremental">

-   '((P ∧ Q) ∨ (Q → R))' is a sentence.
-   '¬¬¬¬¬¬¬¬¬Z' is a sentence.
-   So, by rule 3d, this is also a sentence.

</div>


## Not a Sentence

QQQQR

<div class="incremental">

-   'Q' and 'R' are sentence letters.
-   But there is no way to combine them, using our rules, to get this result.

</div>

## Not a Sentence

\(P)

<div class="incremental">

-   'P' is a sentence.
-   But there is no rule that lets you surround a sentence with parentheses.

</div>

## Not a Sentence

¬\(P)

<div class=incremental>

-   '¬P' is a sentence.
-   But there is no rule that lets you surround a sentence with parentheses.
-   Specifically, rule 2 does not introduce any parentheses.

</div>

## "The Main Connective"

-   (P [→]{.P} Q)
-   [¬]{.P}(P → Q)
-   [¬]{.P}¬¬¬¬¬¬¬¬Z
-   ((P ∧ Q) [∨]{.P} (Q → R))
-   (((P ∧ Q) ∨ (Q → R))[↔]{.P} ¬¬¬¬¬¬¬¬¬Z)

## Parsing in Carnap

[An
example](https://carnap.io/shared/dsanson@gmail.com/Breakout%20Exercise%20Day%2004)

## Breakout Activity

-   Work on the "[Exercises with Official
Notation](https://carnap.io/shared/dsanson@gmail.com/Breakout%20Exercise%20Day%2004#exercises-with-official-notation)"

## Return

Share and Discuss

# Parentheses and Informal Notation

## Outermost Parentheses

  Official    Informal
  ----------- ----------
  (P→Q)       P→Q
  ((P∧Q)∨R)   (P∧Q)∨R
  ¬(P→Q)      Nope

## -Junctions before -ditionals

  Official      Informal
  ------------- ----------
  (P∧Q)→(Q∨R)   P∧Q→Q∨R
  Q↔(R∨S)       Q↔R∨S
  (Q→(R↔S))     Nope

## Comparison to Arithmetic

$2 - 2 \times 2$

<div class="incremental nobullets twocolumn">

-  $2 - (2\times 2)$
-  $2 - 4$
-  $-2$

<!-- -->

-  $(2 - 2) \times 2$
-  $0 \times 2$
-  $0$

</div>

## Comparison to Arithmetic

-  ∧ and ∨ behave kind of like $\times$
-  → and ↔ behave kind of like $+$

## The Lefty Rule for -Junctions

  Official   Informal
  ---------- ----------
  (P∧Q)∧R    P∧Q∧R
  (P∨Q)∨R    P∨Q∨R
  Nope       P∨Q∧R
  Nope       P→Q→R

## Comparison to Arithmetic

$4 - 2 - 2$

<div class="incremental nobullets twocolumn">

-  $(4 - 2) - 2$
-  $2 - 2$
-  $0$

<!-- -->

-  $4 - (2 - 2)$
-  $4 - 0$
-  $4$

</div>

## Breakout Room

-   Go back to [Breakout Exercises page on
Carnap](https://carnap.io/shared/dsanson@gmail.com/Breakout%20Exercise%20Day%2004#exercises-with-informal-notation)
-   Work on the Exercises with Informal Notation

## Return

Share and discuss

# What You Should Be Doing

-   Completing any Retakes on Unit 1
    -   If you haven't taken the Unit 1 Test yet, you are behind.
-   Finishing Unit 2
-   Start in on the Unit 3 Reading over the Weekend
-   Keep talking on Discord.
