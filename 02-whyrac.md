---
layout: page
title: Why RaC?
navigation: 3
---

# When would you use a RaC approach?

Firstly, it is worth saying that there are, broadly speaking, two types of rules (leg/reg or otherwise): prescriptive and judgement-based. 

Prescriptive rules are definitive. For example rules that set thresholds, objective requirements, are numerical or otherwise are not very subjective. Prescriptive rules are not meant to require judgement, but in reality a little interpretation is almost always needed. For example, does "must be over 18" mean from midnight that day, or the end of that day, or from 0+18 years, or 0+17 years, like in countries where people are conssidered 1 at birth versus 0 at birth. In any case, prescriptive rules are most suitable for RaC systems because they help assure consistent application of a rule which is meant to be consistently applied.

Judgement-based rules are ones that require someone accountable to make a judgement. Whether in regulation or legislation, there is a person defined who is directly accountable for the judgement made, which means you should try to preserve the ability for an appropriate person to make a judgement, rather than automating or codifying these rules. Over time judgements accrue, which can provide patterns you can encode, such as "if you meet criteria x, y and z, then the judgement is likely n", but often judgement-based rules are meant to assure actual human judgement, therefore these types of rules are less appropriate for RaC.

There are three key use cases for creating a Rules as Code repository as part of your stack/system:
1. When you need to demonstrate compliance to laws (regulation, legislation) - for instance you may run software for financial institutions, or a company needing to demonstrate environmental compliance, or you are a government department needing to ensure legality of decisions made in your systems (to be compliant to Administrative Law). In any case where you need to demonstrate compliance, it isn't enough to say "we have a compliant system". You need to be able to trace your actions or decisions back to which rules they are compliant with. You can either do this manually, with an army of compliance officers verifying outcomes against the law (which is both expensive and subject to human error or inconsistency), or you can build proactive explainability and compliance into your software. Having the rules you need to comply to available as a utility provides a simplified way to to consume and test against those rules, otherwise compliance becomes a very expensive business, whether in legislation or regulation.
2. When you need to incorporate rules into how your system/service operates - for instance if you want to build a service to help people understand their eligibility to government services, or if you want to create automation of reporting based on regulated triggers (eg, transactions over $10,000), or if you want to create a personalised experience for someone based on rules defined in law or by your organisation. Having rules as a utility helps you ensure you can consume and test against rules without muddying the water with operational policies or system constraints.
3. When you want to design new rules, such as regulation or legislation - Rules as Code helps you model the impact of change from current status to new, and helps you understand the impact more broadly when intersecting with other legislation/regulations. Rules as Code provides a way to run demographic or other bulk data against proposed changes to see whether intended impacts would likely be met, and to identify unintended impacts. It also provides a way to then monitor and measure impact (policy and human) over time, and feed into an interative and agile approach to policy management over time.


# OpenFish Extensions

Going all-in on testing, we consider the broader socio-legal context in that cross-border trade of digital services benefit from consistency. In particular a testbed is extremely valuable for identifying legal mistakes, errors or inconsistenncies between different, but supposedly interoperable, RACs. For example something as simple as "[resident](https://www.oed.com/dictionary/resident_adj?tab=factsheet#25947835)" hits multiple _legal_ and [te ao Māori](## "spiritual worldview") interpretations:
- `ordinarily resident` - intention or fact of establishing a permanent abode (Crimes Act 1961 [§4](https://www.legislation.govt.nz/act/public/1961/0043/194.0/DLM328020.html));
- `habitual resident` - non-permanent or even continuous abode but predominance of activities (NZ-AU DTA 2009 [§4.2](https://www.taxpolicy.ird.govt.nz/-/media/project/ir/tp/tax-treaties/australia/2009-dta-nz-australia-pdf.pdf)
- `tax resident` - subject to govt tarrifs, imposts and [duties](https://www.ird.govt.nz/-/media/project/ir/home/documents/forms-and-guides/ir200---ir299/ir295/ir295.pdf) based on majority of time but alleviated by double-taxation treaties; 
- visa resident = state administered legal _artifact_ that embodies revocable privilege of abode with discretionary work rights;
- ahi kā -  collective linkage to [whenua](## "land and underlying spirtual essence") via proactive maintenance, can be thought of rural Amish with 入土为安.

```diff
! Kei raro i te tarutaru, te tuhi o ngā tū puna 
+ The signs or marks of the ancestors are embedded below the roots of the grass and the herbs
```

<details>
  <summary>because Te Ao Maori worldview ... </summary>
this is is akin to the chinese custom of returning ashes to ancestral motherland so the spirit forms a continuing connection with the clan. Residency is not just the mere physical presence, but the [whakapapa](## "connection/relation") to social group/hierarchy and collective duties to [kaitiaki](## "stewardship or guardianship to locale").  A Golden visa ([investment](https://www.immigration.govt.nz/visas/active-investor-plus-visa/)) might confer pro-forma citizenship at end of migration pathway but an absentee landlord bunkered on a rural [retreat](https://www.mdpi.com/2071-1050/13/15/8161), is fundamentally alien to the community-led principles of [kaitiakitanga](## "relationship to people and country").
</details>

Governments (quite rightly) object to people who gain all the social benefits without a fair contribution to provision of public goods that sustain/subsidise such open society (cf [parachute kid](https://www.oed.com/search/dictionary/?scope=Entries&q=parachute+kid)). This is equating visa residency as paid homestay, rather than invited [kith](https://www.oed.com/dictionary/kith_n?tab=meaning_and_use). Comparative legal research attempts to harmonise definitions, converge to equivalents, and work towards the comity of nations and their legal systems, if not necessarily policies. We can hypothetically model the Treaty of Waitangi as a parallel eco-currency (eco/socio-legal capital as [o ratou taonga katoa](## "treasure and intangibles")) over the EEZ. OpenFISH explores necessary extensions to ground alternative rulesets based on kaitiakitanga as co-regulatory elective regimes.
