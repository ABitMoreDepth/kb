# Zenlike Python

Author: Jason C McDonald
Works for MousePawMedia, Author of Dead Simple Python

Talk about the Zen of python (`import this`)

Codified in PEP-20, the Zen has been around since circa 1999! It wasn't
already considered to be particularly serious.

## Readability Counts
Pythonic code is readable, above all else. Computers don't really care, but
code exists for people.

We write code for other people, and our future selves. We should NOT write
code just to be clever.

"Everyone knows that debugging is twice as hard as writing a program in thee
first place. So if you're as clever as you can be when you write it, how will
you (or the person after you) ever debug it?" - Brian Kernighan, Co-Author of
C.

## Obvious
"There should be one -- and preferably only one -- obvious way to do it."

Usually considered in the context of finding the optimal solution. The
problem is that its usually only obvious once you've found such a solution.

"Why didn't I do it that way the first time?"

## Unless you're Dutch

Typically means: "Obvious in retrospect."

Thing is, we aren't all core developers, so Guido might spot something
quicker than us. However, the "obvious way" can evolve over time.

## Beautiful is better than ugly
Beautiful code is a pleasure to read, typically you'll know it when you see it.

PEP-8 is a good start.

## Explicit
Surprises are bugs-in-waiting.

You can interpret this rule as: "If you need to describe the implementation,
your implementation is wrong."

Typically, comments should describe why something happens, rather than how
something happens.

Take time when naming things. Getting something's name right makes a big
difference in the long term, but can be easy to overlook in the immediate
term.

## Namespaces

`import *` is evil.

Python doesn't support shadowing, so any namespace clashes cause one side of
the clash to be hidden from the implementation.

Finding imports from a wildcard import can be very difficult.

Using `import <module>` is much clearer in intent.

## Refuse to Guess
Guessing leads to bugs. Abtractions are not there to save us thinking, but to
save us typing. We do still need to understand how the code is designed and built.

If its not your code (or even if it is), look it up, read the code as well as
the docs etc. If it is you or your teams code, fix it!

## Simple
Don't be clever.

The "Cleverest" solutions are actually usually the simplest ones, that make
it blindingly obvious how things have been implemented.

Writing simple code is actually harder, than writing complex code.

## Complex is better than complicated
Not everything is simple

Elegance is NOT Obfuscation.

Complex code takes more time to read, but should not take more effort.  Complex should still be "pythonic".

## Easy to Explain
If the implementation is hard to explain, its a bad idea.

Simple, or at least complex means it should be obvious to the reader. Not all
simple code is good, though all good code is simple (or reasonably complex).
Not all obvious code is good either.

## Flat
Flat is better than nested.

Nesting is hard to follow, and its very easy to get nesting wrong (in code,
not data).

## Sparse
Sparse is better than dense.  

Mozart: "The music is not in the notes, but in the silence between."

The same is true in code.  Whitespace helps us to logically organise the code.

Beware of complex one-liners.

## Errors
An Error is an exceptional state. Typically this means we need to do
something to handle that state, or bail out of the program.

If we don't handle an exception, then things will likely only get worse.

For gods sake, DON'T silence errors.  Either let them explode, or handle them.

### Explicitly Silenced
Caveat to the above, unless you've already handled the exception behaviour.
Try to ensure that you only silence the most specific error cases you can,
again DON'T silence all errors.

## Now
Now is better than never.

The longer you leave it, the more likely you either won't be able to, or you
won't get around to it.

If you really can't get to something right now, at least try to pave the way
for future you.

## never
The other issue is, never is often better than *right* now.

Its important to prioritise what is needed and what is not, when trying to
determine whether to implement something immediately or not.

## Special cases
Its not really possible to bend away from standards all the time, but
sometimes, there really is no alternative. However, its important not to lose
the meaning and significance of breaking a standard.

Typically, its worth commenting inline with the implementation to clarify
exactly why you've had to make an exception from a standard.

## The Zen is eternally unfinished
Tim Peters left a 20th spot in the zen for Guido to fill in at some point in
the future, which to date, has not happened.

In a way, its a nice thing to leave it unfilled, as python has not ceased to
continue evolving, which somewhat fits nicely.

---

### Links:
- PEP-8
- [[python]]


[//begin]: # "Autogenerated link references for markdown compatibility"
[python]: python "Python"
[//end]: # "Autogenerated link references"