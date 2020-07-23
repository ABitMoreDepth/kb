# Effective Code Reviews

Unsurprisingly, code review is hard...

## Why do code reviews?
- Knowledge Transmission (Bus Factor)
- Stimulate collective collaboration
- Quick feedback / Ensure changes are on the right track
- Stimulate contribution for new PRs and to maintain good practices
- Ensure we maintain good quality ~~code~~ product

## Rules for healthy code reviews
- Don't take any comments personally.
- Listen to feedback - Many people struggle to incorporate feedback from others.
- Accept the fact you may be wrong.  Making mistakes is a core part of being human.

## Good practices
- Don't forget to leave positive feedback, its all too easy to forget to
praise good work and only comment on areas that need improvement.
- Use emoji's/memes in areas where you wish to make a possibly contentious
comment but wish to maintain a congenial tone.

### What metrics should we use when analysing a PR?
- Its tough to provide a single list thats good, but one way to look at a PR
is how many curse words vs complimentary words that float through your brain
when reviewing the PR.
- Sometimes you can keep an eye on the code legibility, does it have comments
where needed, does it make use of appropriate variable names and code
structure?
- Does the PR actually achieve the goal its meant to?
  
### Negative Feedback
- Always be nice.  Have empathy with the author
- Use collective words (us, can we, all) instead of individual terms (I, you, him).
- Be clear and straight to the point (whilst being nice). If its hard to get
a point across in text, arrange to discuss feedback over a call/face-to-face

## Checklist - During Development
- Is your PR getting large? Ideally keep actual logical changes to < 250 -
400 lines of code. (Sometimes this is not easily achievable)
- There's nothing wrong with raising a PR early and marking it as a WIP.
  - Sometimes this can help you avoid a pitfall, if a colleague/reviewer spots
   you heading in the wrong direction. 
- Put style changes into independant commits - These changes are easily
automated and usually don't invole logical changes, so it makes sense to
separate them.

## Checklist - Prior to opening a PR
- Review your own PR before giving it to others
- Check your tests pass and your changes meet style guides before requesting review.
- Is the PR Title & description clear?

## Checklist - reviewing
- If the tests or build pipeline are failing, don't review any further.
- Typos - Comments, tests, variable names, classes etc.
- Words in non-codebase languages (most codebases are written in english,
  even if Authors don't always speak English as a first language)
- Logic errors (the meat)
- Performance optimisations - but be careful of encouraging optimisation too
  early in the development process
- Follow style conventions, architectural conventions & team best practices
- Ensure Commit messages are in line with the project standards

---

### Links
- 