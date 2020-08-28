---
css: 
-   https://www.davidsanson.com/css/tufte.css
-   https://www.davidsanson.com/css/tuftextra.css
-   https://www.davidsanson.com/css/carnap.css
js: https://www.davidsanson.com/js/carnap.js
---

# Breakout Exercises, Day 04

These are all exercises designed to help you become more comfortable parsing
symbolic sentences in SL. They are not for points, just practice.

## An Example for Us to Complete Together


For typing in symbols, use this shorthand:

 Connective           Keyboard Shorthand 
------------         --------------------
  $\land$            /\\
  $\lor$             \\/
  $\rightarrow$      -> 
  $\leftrightarrow$  <->
  $\neg$             ~

~~~{.SynChecker .Match submission=none}
BRE4.0 (P->~Q)/\(R<>~S)
~~~


## Exercises with Official Notation

1.  Every sentence letter '$\mathrm{P}$', '$\mathrm{Q}$', '$\mathrm{R}$', ...,
    '$\mathrm{Z}$' is a sentence. And so are the sentence letters with
    subscripts.
2.  If '$\mathrm{▢ }$' is a sentence, then '$\mathrm{\mathord{\neg} ▢ }$' is too.
3.  If '$\mathrm{▢ }$' and '$\mathrm{◯ }$' are both sentences, then:
    a.  '$\mathrm{(▢ \mathbin{\wedge} ◯ )}$' is also a sentence, and
    b.  '$\mathrm{(▢ \mathbin{\vee} ◯ )}$' is also a sentence, and
    c.  '$\mathrm{(▢ \mathbin{\rightarrow} ◯ )}$' is also a sentence, and
    d.  '$\mathrm{(▢ \mathbin{\leftrightarrow} ◯ )}$' is also a sentence.

Each of the following is a well-formed sentence, according to these rules.
Parse them:

```{.SynChecker .Match submission=none}
BRE4.1 ~~~~~~~~~~~~~~~~~~~~P
BRE4.2 ~(P\/Q)
BRE4.3 (P\/Q)/\R->S/\T
BRE4.4 (((P\/Q)/\R)->S)/\T
BRE4.5 (R->S)->S
```

Each of the following is not a sentence, according to our rules. *Try* to
parse them, and think about why they cannot be built up using our rules.

@.   PP

<textarea style="height: 5em">
</textarea>

@.   P→Q

<textarea style="height: 5em">
</textarea>

@.   (¬P)

<textarea style="height: 5em">
</textarea>

@.   (P∨Q∨R)

<textarea style="height: 5em">
</textarea>

@.   (P∨(Q∧R)∨S)

<textarea style="height: 5em">
</textarea>

## Exercises with Informal Notation

Informal Notation is when we drop parentheses according to our three
conventions:

Drop Outermost Parentheses
:   If a sentence in official notation has outermost parentheses, you can drop
    those parentheses.

-junctions Before -ditionals
:   -junctions group more tightly than -ditionals. 

The Lefty Rule for -junctions
:   Sequences of adjacent conjunctions, and sequences of adjacent
    disjunctions, (but not sequences that mix both together) group to the left.

Parse these sentences that are written in informal notation:

```{.SynChecker .MatchClean submission=none}
BRE4.6 P/\Q/\R/\S/\T
BRE4.7 P/\Q/\(R/\(S/\T))
BRE4.8 ~P->Q
BRE4.9 ~(P->Q)
BRE4.10 P->Q/\R
BRE4.11 P/\Q->R
BRE4.12 P/\Q<>Q/\R
```

Here are some sequences of symbols that are not sentences, even in our
informal notation. Try to explain why.


@.   P∧Q∨R∧S

<textarea style="height: 5em">
</textarea>

@.   P→Q→R→S

<textarea style="height: 5em">
</textarea>

@.   ((P∧Q))∧R∧S

<textarea style="height: 5em">
</textarea>

@.   ~(P↔Q↔R)

<textarea style="height: 5em">
</textarea>

@.   A→B  

<textarea style="height: 5em">
</textarea>
