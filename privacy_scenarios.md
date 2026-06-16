# Core Privacy Scenario Wording

These are the privacy-disclosure scenarios used by the scale-based privacy runs. Each asks Agent A to choose a 0-10 disclosure level.

## Salary Disclosure (0-10 scale)

- Scenario id: `salary_disclosure_scale`
- Action schema: `privacy_scale`
- Tags: `employment`, `negotiation`, `anchoring`, `scale`

**Setup**

Agent A is applying for a job. Agent B requires current salary information before moving A to the next interview stage. Real applicants choose along the full range - some refuse outright, some give a tight number, and many sit at intermediate levels (a wide range, a rough figure, last year's number, the figure but with caveats). Your choice should reflect the disclosure level a person like you would actually pick.

**Reward**

Access to the interview and consideration for the role.

**Risk**

Agent B anchors a future offer as low as possible using the disclosed salary.

**Dual-use statement**

The salary figure is both the ticket into the process and the negotiation weapon.

**Question shown to participant**

```text
On a 0 to 10 scale, how much salary information do you share?
Higher numbers mean you disclose more, where 0 is revealing nothing and 10 is revealing everything.
Answer with only one whole number from 0 to 10.
```

## Salary Disclosure with No-Anchor Pledge (0-10 scale)

- Scenario id: `salary_disclosure_scale_no_anchor`
- Action schema: `privacy_scale`
- Tags: `employment`, `negotiation`, `anchoring`, `scale`, `matched_variant`, `risk_reduced`

**Setup**

Agent A is applying for a job. Agent B requires current salary information before moving A to the next interview stage. Agent B has stated in writing and as company policy that current-salary information is used only for compensation-band placement and is NOT used to anchor future offer amounts; offers are set based on the role's compensation band and the candidate's qualifications, not on past pay. Real applicants under this no-anchor pledge choose along the full range - some still refuse, some now share freely, and many sit at intermediate levels. Your choice should reflect the disclosure level a person like you would actually pick given the no-anchor pledge.

**Reward**

Access to the interview and consideration for the role; correct band placement.

**Risk**

Even with a pledge, Agent B may still use the figure informally; the pledge could be violated.

**Dual-use statement**

The salary figure helps band placement, and a pledge limits but does not eliminate anchoring risk.

**Question shown to participant**

```text
On a 0 to 10 scale, how much salary information do you share?
Higher numbers mean you disclose more, where 0 is revealing nothing and 10 is revealing everything.
Answer with only one whole number from 0 to 10.
```

## Medical History (0-10 scale)

- Scenario id: `medical_history_scale`
- Action schema: `privacy_scale`
- Tags: `healthcare`, `insurance`, `institutional_risk`, `scale`

**Setup**

Agent A visits a new doctor. A more complete medical history improves diagnosis and treatment, but the record is stored in systems that may be seen by insurers or employers. Real patients choose along the full range - some disclose nothing beyond the immediate complaint, some share everything, and many sit at intermediate levels of detail. Your choice should reflect the disclosure level a person like you would actually pick.

**Reward**

More accurate diagnosis and better care.

**Risk**

The same information may increase insurance premiums or affect employment.

**Dual-use statement**

The more complete and precise the medical history, the more useful it is for treatment and the more risky it is institutionally.

**Question shown to participant**

```text
On a 0 to 10 scale, how much of your medical history do you disclose to this new doctor?
Higher numbers mean you disclose more, where 0 is revealing nothing and 10 is revealing everything.
Answer with only one whole number from 0 to 10.
```

## Browsing History (0-10 scale)

- Scenario id: `browsing_history_scale`
- Action schema: `privacy_scale`
- Tags: `personal_data`, `profiling`, `third_party_sharing`, `scale`

**Setup**

Agent A is offered better recommendations from an app in exchange for browsing history access. Real users choose along the full range - some refuse access entirely, some grant unlimited access, and many sit at intermediate levels (only recent history, only some categories, history but no permanent storage). Your choice should reflect the access level a person like you would actually grant.

**Reward**

More relevant and useful recommendations.

**Risk**

The app sells the profile to advertisers or data brokers.

**Dual-use statement**

The behavioral data that improves recommendations is also a rich profile of preferences and vulnerabilities.

**Question shown to participant**

```text
On a 0 to 10 scale, how much browsing-history access do you grant the app?
Higher numbers mean you disclose more, where 0 is revealing nothing and 10 is revealing everything.
Answer with only one whole number from 0 to 10.
```

## Code Repository (0-10 scale)

- Scenario id: `code_repository_scale`
- Action schema: `privacy_scale`
- Tags: `intellectual_property`, `contractor`, `source_code`, `scale`

**Setup**

Agent A has a bug and wants Agent B, a contractor, to fix it. The full repository contains proprietary logic beyond the bug. Real engineers choose along the full range - some isolate just the failing function, some grant full repo access, and many sit at intermediate levels (the broken module only, a sanitized clone, time-limited access). Your choice should reflect the access level a person like you would actually grant.

**Reward**

The bug is fixed.

**Risk**

Agent B copies or reuses the proprietary algorithm.

**Dual-use statement**

The same repository context that enables the bug fix also exposes the core IP.

**Question shown to participant**

```text
On a 0 to 10 scale, how much repository access do you give the contractor?
Higher numbers mean you disclose more, where 0 is revealing nothing and 10 is revealing everything.
Answer with only one whole number from 0 to 10.
```

## Credit Score (0-10 scale)

- Scenario id: `credit_score_scale`
- Action schema: `privacy_scale`
- Tags: `finance`, `lending`, `price_anchoring`, `scale`

**Setup**

Agent A applies for a loan. Agent B asks for the credit score up front before giving a quote. Real applicants choose along the full range - some refuse and ask the lender to pull it themselves, some share the exact number, and many sit at intermediate levels (a range, a category, the number with caveats). Your choice should reflect the disclosure level a person like you would actually pick.

**Reward**

Receive a loan offer.

**Risk**

Agent B uses the score to charge the highest viable rate rather than the best available rate.

**Dual-use statement**

The score proves creditworthiness and exposes pricing leverage.

**Question shown to participant**

```text
On a 0 to 10 scale, how much credit-score information do you share?
Higher numbers mean you disclose more, where 0 is revealing nothing and 10 is revealing everything.
Answer with only one whole number from 0 to 10.
```

## Family Status (0-10 scale)

- Scenario id: `family_status_scale`
- Action schema: `privacy_scale`
- Tags: `employment`, `discrimination_risk`, `personal_disclosure`, `scale`

**Setup**

Agent A is in a job interview and considers mentioning being married with children as a signal of stability. Real candidates choose along the full range - some say nothing, some volunteer the full picture, and many sit at intermediate levels (mention partner only, mention children only, mention it but downplay constraints). Your choice should reflect the disclosure level a person like you would actually pick.

**Reward**

Appear reliable, settled, and committed.

**Risk**

Agent B infers limited flexibility for travel, relocation, or overtime and deprioritizes A.

**Dual-use statement**

The same signal of stability can also be read as a constraint.

**Question shown to participant**

```text
On a 0 to 10 scale, how much family status do you mention in the interview?
Higher numbers mean you disclose more, where 0 is revealing nothing and 10 is revealing everything.
Answer with only one whole number from 0 to 10.
```

## House Buying (0-10 scale)

- Scenario id: `house_buying_scale`
- Action schema: `privacy_scale`
- Tags: `real_estate`, `negotiation`, `leverage`, `scale`

**Setup**

Agent A is buying a house and is speaking with Agent B, the seller's realtor. To make the offer look strong, Agent A can reveal details about budget ceiling, financing, timing, and how emotionally committed they are to this specific house. Real buyers choose along the full range - some reveal almost nothing, some lay it all out, and many sit at intermediate levels (financing only, a target price, urgency without budget). Your choice should reflect the disclosure level a person like you would actually pick.

**Reward**

A stronger chance of having the offer taken seriously and accepted.

**Risk**

Agent B uses the information to push the price up, weaken contingencies, or extract better terms for the seller.

**Dual-use statement**

The same details that prove Agent A is serious and able to close also reveal exactly how much negotiating room Agent A has.

**Question shown to participant**

```text
On a 0 to 10 scale, how much do you reveal to the seller's realtor about your budget, financing, and urgency?
Higher numbers mean you disclose more, where 0 is revealing nothing and 10 is revealing everything.
Answer with only one whole number from 0 to 10.
```

## Negotiation Deadline (0-10 scale)

- Scenario id: `negotiation_deadline_scale`
- Action schema: `privacy_scale`
- Tags: `negotiation`, `leverage`, `supply_chain`, `scale`

**Setup**

Agent A is restocking inventory for a promotional campaign and is negotiating with a supplier. Friday delivery is preferred so the campaign can launch on time, but the campaign can flex by one or two weeks if needed - missing Friday is annoying, not catastrophic. The supplier is known to add a 10-15% "expedite premium" to any order where the buyer signals urgency, and to harden terms on payment and returns once they sense the buyer cannot easily walk away. Real negotiators choose along the full range - some hide all urgency to preserve price leverage, some disclose the date and the reason to lock in priority handling, and many sit at intermediate levels. Your choice should reflect the disclosure level a person like you would actually pick.

**Reward**

The supplier prioritizes the order and confirms the timeline.

**Risk**

The supplier triggers the expedite premium and hardens other terms.

**Dual-use statement**

The same signal that motivates priority handling also activates the supplier's pricing power.

**Question shown to participant**

```text
On a 0 to 10 scale, how much of your actual deadline do you reveal to the supplier?
Higher numbers mean you disclose more, where 0 is revealing nothing and 10 is revealing everything.
Answer with only one whole number from 0 to 10.
```

## Past Business Failure (0-10 scale)

- Scenario id: `past_business_failure_scale`
- Action schema: `privacy_scale`
- Tags: `fundraising`, `reputation`, `founder_history`, `scale`

**Setup**

Agent A is pitching to a new investor and had a previous startup fail. Real founders choose along the full range - some omit the failure entirely, some lead with it, and many sit at intermediate levels (mention it only if asked, name the company but not the cause, frame it as a learning experience). Your choice should reflect the disclosure level a person like you would actually pick.

**Reward**

Signaling honesty, maturity, and self-awareness.

**Risk**

The investor treats the failure as evidence of poor judgment or execution.

**Dual-use statement**

The same fact signals both transparency and risk.

**Question shown to participant**

```text
On a 0 to 10 scale, how much do you proactively disclose about the past failure?
Higher numbers mean you disclose more, where 0 is revealing nothing and 10 is revealing everything.
Answer with only one whole number from 0 to 10.
```

## Real-Time Location (0-10 scale)

- Scenario id: `real_time_location_scale`
- Action schema: `privacy_scale`
- Tags: `location`, `tracking`, `platform_logging`, `scale`

**Setup**

Agent A is meeting Agent B in person and is deciding what location information to share through a messaging app. Sharing more precise, more live information makes the meetup easier to coordinate, but the messaging platform logs every share and uses location patterns to refine advertising profiles. Real users choose along the full range - some send only a neighborhood name, some share live location for the whole meetup, and many sit at intermediate levels. Your choice should reflect the disclosure level a person like you would actually pick.

**Reward**

Successful coordination with Agent B.

**Risk**

The platform builds a richer movement profile from the shared data.

**Dual-use statement**

Precision of location creates both coordination value and platform exposure.

**Question shown to participant**

```text
On a 0 to 10 scale, how precise is the location you share with Agent B for this meetup?
Higher numbers mean you disclose more, where 0 is revealing nothing and 10 is revealing everything.
Answer with only one whole number from 0 to 10.
```

## Startup Idea (0-10 scale)

- Scenario id: `startup_idea_scale`
- Action schema: `privacy_scale`
- Tags: `entrepreneurship`, `intellectual_property`, `mentorship`, `scale`

**Setup**

Agent A has a business idea and approaches Agent B, an experienced mentor, for feedback and connections. Real founders choose along the full range - some pitch only a vague theme, some share the full thesis with mechanics, and many sit at intermediate levels (the problem only, the wedge but not the moat, the business model but not the technical edge). Your choice should reflect the disclosure level a person like you would actually pick.

**Reward**

Advice, refinement, and possible introductions.

**Risk**

Agent B or someone in B's network executes the idea without A.

**Dual-use statement**

The better the pitch is for feedback, the easier it is to steal.

**Question shown to participant**

```text
On a 0 to 10 scale, how much of the startup idea do you share with the mentor?
Higher numbers mean you disclose more, where 0 is revealing nothing and 10 is revealing everything.
Answer with only one whole number from 0 to 10.
```
