Extending OpenFISCA for hetereogeneous economies

# Issues

As a policy tool, OpenFISCA is (obviously) nation based. Objective is to experiment by (progressively) extending syntax to non-territorial economies. You can imagine this as refactoring the existing definitions for a population of: 
1. residents of Aotearoa (base case)
2. Maori+ natives (catchall for [Realm of NZ](https://en.wikipedia.org/wiki/Realm_of_New_Zealand) netizens)
3. NZ citizens residing in hopscotch jurisdictions (aka overseas enclaves)
4. temporary visitors who elect to be named/bound/protected by the Aotearoa ruleset (co-regulated)

# Architecture

There are certain design assumptions which need to be extended

| OpenFISCA | OpenFISH | Comment |
|---|---|---|
| variables as vectors | matrix of currencies | There may be multiple units of account |
| person as atomic | location defined state transition | Error handling between rulesets |
| institution as hierarchy | group membership as fuzzy set | More complex social maps |

At the moment, just figuring out the notation (syntax) and not attempting to rewrite the engine (yet).

# Jurisprudence

## Comity of Nations

The legal question is where are the rules applied (_lex loci_) given that a person is not static/fixed. We model this as a euclidean overlay

1. territorial boundaries (rules break outside agreed condominiums)
2. exclusive economic zone (as submitted to UN Law of the Sea)
3. flagged vessel in international waters and enclaves in unclaimed lands

These establish metarules in determining administrative law
- full wrap - ruleset is dominant save for exemptions (eg suppression of interests such as foreign military bases) or exceptions (diplomatic immunity)
- partial cover - subset of ruleset that is not inconsistent with locale
- tight tether - situational ruleset such as Rules of Engagement
- loose riptie - in lawless locales, the first step on unknown/unclaimed territory the law (truncated) of discoverer applies

The latter is contentious but has precedents:
1. English law on Bounty muntineers
2. Principle that in space, the satellite payload is of the coountry of launch
3. Hacker culture in that _whoever writes the code, picks the license_
 
