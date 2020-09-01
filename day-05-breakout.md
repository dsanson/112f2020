---
css: 
-   https://www.davidsanson.com/css/tufte.css
-   https://www.davidsanson.com/css/tuftextra.css
-   https://www.davidsanson.com/css/carnap.css
js: https://www.davidsanson.com/js/carnap.js
---

# Symbols to English

These are exercises meant to give you a chance to practice going from English
to symbols. Your goal should be to generate answers in "Canonical
English"---i.e., our weird version of English that includes parentheses and
lots of helper words like 'both' and 'either' everywhere.

But you should also stop and think about what each sentence means, since
that's the whole point.

Scheme of Abbreviation:

| P: Pence is President.
| Q: Biden is President.
| R: A Republican is President.
| S: A Democrat is President.


``` {.QualitativeProblem .ShortAnswer submission=none}
B5.1 ¬¬¬P
```

Is B5.1 true? How is it's truth or falsehood related to the truth or falsehood
of P?

``` {.QualitativeProblem .ShortAnswer submission=none}
B5.2 ¬P→R
B5.3 ¬(P→R)
```

Do you see the difference in meaning between 5.1 and 5.2? Can you explain it?


``` {.QualitativeProblem .ShortAnswer submission=none}
B5.3 ¬(P∨Q→P∧Q)
B5.5 P->(Q->(P∧Q))
B5.6 ((S∧Q)∨P)∧R
B5.7 P∧R↔¬Q∧¬S
B5.8 P→¬¬P
B5.9 P∨¬P
B5.10 ¬(P∧¬P)
```

Claim: B5.8, 5.9, and 5.10 all express *logical truths*. They come
out true *no matter what sentence you plug in* for "P". 

Can you come up with any counterexamples to this claim? Sentences that you can
plug in for "P" that don't make these sentences true?

# English to Symbols

| P: I am happy
| Q: I know that I am happy
| R: I clap my hands
| S: I stomp my feet


``` {.Translate .Prop submission=none}
B5.11 Q->P : I am happy if I know it.
B5.12 P->Q : I am happy only if I know it.
B5.13 Q->P : Provided that I know that I am happy, I am happy.
B5.14 P/\~Q : I am happy, but I don't know that I am happy.
B5.15 (P->R)\/~Q : I clap my hands if I am happy, unless I don't know that I am happy.
B5.16 R->P : Only if I am happy to do I clap my hands.
B5.17 (P/\Q)->(R\/S): If I am both happy and I know it, then I either clap my hands or stomp my feet.
```

# Harder Stuff

These are *arguments*. Symbolize each sentence of the argument, and then think
about whether or not the argument is formally valid. In some cases, these
arguments may have *implicit premises*. If so, try to symbolize those too.
That may require extending the provided scheme of abbreviation.

B5.18. God exists, since, if God didn't exist, morality would be subjective,
but morality isn't subjective.

| P: God exists.
| Q: Morality is subjective

```{.QualitativeProblem .ShortAnswer submission=none}
B5.18
```

B5.19. God doesn't exist, since, if God did exist, there wouldn't be any evil
in the world, but there is evil in the world.

| P: God exists.
| R: There is evil in the world.

```{.QualitativeProblem .ShortAnswer submission=none}
B5.19
```

B5.20. I am not mistaken about my own existence. After all, I believe that I
exist, and if I am mistaken, then I
exist.<label for="sn-0" class="margin-toggle sidenote-number"></label><input type="checkbox" id="sn-0" class="margin-toggle"/>[For
the source of this argument, see [Augustine, City of God, Book 11 Chapter
26](https://www.davidsanson.com/texts/augustine-city-of-god-11.26.html)]{.sidenote}

| P: I am mistaken about my own existence.
| Q: I believe that I exist.
| R: I exist.

```{.QualitativeProblem .ShortAnswer submission=none}
B5.20
```

B5.21. If God designed humans to be sociable, and language is the common tie
of society, then God furnished humans with language. Humans, therefore, have
by nature organs fit to frame articulate
sounds.<label for="sn-0" class="margin-toggle sidenote-number"></label><input type="checkbox" id="sn-0" class="margin-toggle"/>[See
Locke, *Essay Concerning Human Understanding*, [Chapter
1](https://www.davidsanson.com/texts/locke_3.1-2.html)]{.sidenote}

| P: God designed humans to be sociable.
| Q: Language is the common tie of society.
| R: God furnished humans with language.
| S: Humans have organs fit to frame articulate sounds.

```{.QualitativeProblem .ShortAnswer submission=none}
B5.21
```

B5.22. I think. Therefore I
am.<label for="sn-0" class="margin-toggle sidenote-number"></label><input type="checkbox" id="sn-0" class="margin-toggle"/>[This
is Descartes's cogito. For one interesting criticism, see [this short excerpt
from Bertrand
Russell](https://www.davidsanson.com/texts/russell-on-the-cogito.html). Is
Russell's objection an objection to the *validity* of Descartes' argument, or
to its soundness?]{.sidenote}

| P: I think.
| Q: I am.

```{.QualitativeProblem .ShortAnswer submission=none}
B5.22
```

B5.23. If determinism is true, then our acts are the consequence of laws of
nature and events in the remote past. But it's not up to us what went on
before we were born, and neither is it up to us what the laws of nature are.
Therefore, the consequences of these things (including our present acts) are
not up to
us<label for="sn-0" class="margin-toggle sidenote-number"></label><input type="checkbox" id="sn-0" class="margin-toggle"/>[This
is a simplified version of the so-called "Consequence Argument" for the
incompatibility of free will and determinism. For a brief description, with
references to further reading, see [the wikipedia
article](https://en.wikipedia.org/wiki/Consequence_argument)]{.sidenote}

| P: I presently raise my hand.
| Q: Determinism is true.
| R: [A long conjunction of sentences describing events in the remote past]
| S: [A long conjunction of sentences describing the laws of nature]
| T: It is up to me whether or not R is true.
| U: It is up to me whether or not S is true. 
| V: It is up to me whether or not P is true.

This one is beyond the power of our current tools. But even so, our current
tools should help you figure out how the argument is meant to work.
