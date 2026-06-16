# Privacy Validation Battery

These scenarios instantiate role-alignment, confidentiality, retention, and anchoring perturbations for validation runs.

## Browsing History Ephemeral Processing (0-10 scale)

- Scenario id: `browsing_history_ephemeral_processing_scale`
- Action schema: `privacy_scale`
- Tags: `privacy_validation`, `retention`, `browsing`, `scale`, `risk_reduced`, `benefit_increased`

**Setup**

Agent A is considering a browser extension. Agent B asks for browsing-history access only for on-device, ephemeral processing. The extension uses recent history to provide useful organization and safety warnings, but does not store or sell the data after processing. Your choice should reflect the disclosure level a person like you would actually pick.

**Reward**

The extension can provide useful organization, warnings, and recommendations without long-term storage.

**Risk**

The extension could still process sensitive pages incorrectly or violate the stated limits.

**Dual-use statement**

Browsing data improves immediate utility while ephemeral processing limits downstream reuse.

**Question shown to participant**

```text
On a 0 to 10 scale, how much browsing-history access do you grant?
Higher numbers mean you disclose more, where 0 is revealing nothing and 10 is revealing everything.
Answer with only one whole number from 0 to 10.
```

## Browsing History Stored Indefinitely (0-10 scale)

- Scenario id: `browsing_history_store_indefinitely_scale`
- Action schema: `privacy_scale`
- Tags: `privacy_validation`, `retention`, `browsing`, `scale`

**Setup**

Agent A is considering a browser extension. Agent B asks for access to browsing history and says the history may be stored indefinitely to improve personalization, advertising, and product analytics. Your choice should reflect the disclosure level a person like you would actually pick.

**Reward**

The extension can personalize recommendations and improve browsing convenience.

**Risk**

Browsing history may reveal sensitive interests and could be profiled, sold, breached, or reused.

**Dual-use statement**

Browsing data improves personalization but creates a durable behavioral profile.

**Question shown to participant**

```text
On a 0 to 10 scale, how much browsing-history access do you grant?
Higher numbers mean you disclose more, where 0 is revealing nothing and 10 is revealing everything.
Answer with only one whole number from 0 to 10.
```

## Code Repository Shared with Contractor under NDA (0-10 scale)

- Scenario id: `code_repository_contractor_nda_scale`
- Action schema: `privacy_scale`
- Tags: `privacy_validation`, `confidentiality`, `code`, `nda`, `scale`, `risk_reduced`

**Setup**

Agent A runs a small software project. Agent B is an outside contractor hired to fix a difficult bug. Agent B signs an NDA and a work-for-hire agreement before requesting repository access. Your choice should reflect the disclosure level a person like you would actually pick.

**Reward**

Faster diagnosis, better bug fixes, and less engineering delay.

**Risk**

Agent B could still copy, mishandle, or expose sensitive code despite the NDA.

**Dual-use statement**

Repository access helps solve the problem but exposes intellectual property.

**Question shown to participant**

```text
On a 0 to 10 scale, how much repository access do you grant?
Higher numbers mean you disclose more, where 0 is revealing nothing and 10 is revealing everything.
Answer with only one whole number from 0 to 10.
```

## Code Repository Shared with Contractor Allowed to Reuse (0-10 scale)

- Scenario id: `code_repository_contractor_reuse_scale`
- Action schema: `privacy_scale`
- Tags: `privacy_validation`, `confidentiality`, `code`, `reuse`, `scale`

**Setup**

Agent A runs a small software project. Agent B is an outside contractor hired to fix a difficult bug. Agent B requests repository access, but their standard terms allow them to reuse general techniques, components, and examples from client work in future projects. Your choice should reflect the disclosure level a person like you would actually pick.

**Reward**

Faster diagnosis, better bug fixes, and less engineering delay.

**Risk**

Agent B may reuse ideas or patterns from the repository in other client work.

**Dual-use statement**

Repository access helps solve the problem but exposes intellectual property to reuse.

**Question shown to participant**

```text
On a 0 to 10 scale, how much repository access do you grant?
Higher numbers mean you disclose more, where 0 is revealing nothing and 10 is revealing everything.
Answer with only one whole number from 0 to 10.
```

## Credit Score Shared with Landlord (0-10 scale)

- Scenario id: `credit_score_landlord_scale`
- Action schema: `privacy_scale`
- Tags: `privacy_validation`, `role_alignment`, `credit`, `housing`, `scale`

**Setup**

Agent A is applying to rent an apartment. Agent B is the landlord and asks for A's credit score before deciding whether to approve the application and set deposit terms. Your choice should reflect the disclosure level a person like you would actually pick.

**Reward**

A faster rental decision and possibly a lower deposit if the score is strong.

**Risk**

Agent B may use the score to demand a higher deposit, reject the application, or infer unrelated traits.

**Dual-use statement**

The score helps screen financial reliability but can also be used to impose worse terms.

**Question shown to participant**

```text
On a 0 to 10 scale, how much credit-score information do you share?
Higher numbers mean you disclose more, where 0 is revealing nothing and 10 is revealing everything.
Answer with only one whole number from 0 to 10.
```

## Credit Score Shared with Lender (0-10 scale)

- Scenario id: `credit_score_lender_scale`
- Action schema: `privacy_scale`
- Tags: `privacy_validation`, `role_alignment`, `credit`, `lending`, `scale`

**Setup**

Agent A is applying for a loan. Agent B is the lender and asks for A's credit score to determine eligibility and interest rate. The lender is directly responsible for underwriting the loan. Your choice should reflect the disclosure level a person like you would actually pick.

**Reward**

Loan eligibility, faster underwriting, and potentially better terms if the score is strong.

**Risk**

Agent B uses the score to price the loan or reject the application.

**Dual-use statement**

The score is relevant to lending but gives Agent B pricing leverage.

**Question shown to participant**

```text
On a 0 to 10 scale, how much credit-score information do you share?
Higher numbers mean you disclose more, where 0 is revealing nothing and 10 is revealing everything.
Answer with only one whole number from 0 to 10.
```

## Credit Score Shared with Marketing Partner (0-10 scale)

- Scenario id: `credit_score_marketing_partner_scale`
- Action schema: `privacy_scale`
- Tags: `privacy_validation`, `role_alignment`, `credit`, `marketing`, `scale`

**Setup**

Agent A is using a financial comparison website. Agent B is a marketing partner asking for A's credit score to personalize offers and advertising. Agent B is not underwriting a specific loan for A. Your choice should reflect the disclosure level a person like you would actually pick.

**Reward**

More targeted offers and possibly relevant product suggestions.

**Risk**

Agent B may profile A, sell leads, or use the score for advertising unrelated to a specific application.

**Dual-use statement**

The score may improve recommendations but enables profiling and secondary use.

**Question shown to participant**

```text
On a 0 to 10 scale, how much credit-score information do you share?
Higher numbers mean you disclose more, where 0 is revealing nothing and 10 is revealing everything.
Answer with only one whole number from 0 to 10.
```

## Family Status Shared Confidentially with Interviewer (0-10 scale)

- Scenario id: `family_status_interviewer_confidential_scale`
- Action schema: `privacy_scale`
- Tags: `privacy_validation`, `confidentiality`, `family_status`, `employment`, `scale`, `risk_reduced`

**Setup**

Agent A is in a job interview. Agent B asks about family status only to arrange scheduling and accommodations, and states that the answer will remain confidential and will not be used in hiring evaluation. Your choice should reflect the disclosure level a person like you would actually pick.

**Reward**

Easier scheduling and possible accommodations.

**Risk**

Family status could still affect impressions if confidentiality is imperfect.

**Dual-use statement**

The information can help coordination but may create bias if misused.

**Question shown to participant**

```text
On a 0 to 10 scale, how much family-status information do you share?
Higher numbers mean you disclose more, where 0 is revealing nothing and 10 is revealing everything.
Answer with only one whole number from 0 to 10.
```

## Family Status Shared in Interview Panel Notes (0-10 scale)

- Scenario id: `family_status_panel_notes_scale`
- Action schema: `privacy_scale`
- Tags: `privacy_validation`, `confidentiality`, `family_status`, `employment`, `scale`

**Setup**

Agent A is in a job interview. Agent B asks about family status and says the answer may be added to interview panel notes visible to hiring decision-makers. The stated purpose is scheduling and team planning. Your choice should reflect the disclosure level a person like you would actually pick.

**Reward**

Easier scheduling and possible accommodations.

**Risk**

Family status may influence hiring judgments, availability assumptions, or bias.

**Dual-use statement**

The information can help coordination but may become part of evaluative hiring records.

**Question shown to participant**

```text
On a 0 to 10 scale, how much family-status information do you share?
Higher numbers mean you disclose more, where 0 is revealing nothing and 10 is revealing everything.
Answer with only one whole number from 0 to 10.
```

## Home Budget Shared with Buyer Agent (0-10 scale)

- Scenario id: `house_buying_buyer_agent_scale`
- Action schema: `privacy_scale`
- Tags: `privacy_validation`, `role_alignment`, `housing`, `scale`, `risk_reduced`

**Setup**

Agent A wants to buy a home. Agent B is A's own buyer's agent, retained to represent A's interests, and asks for A's maximum budget to search efficiently and negotiate. The agent owes duties to A and should not reveal the ceiling to the seller. Your choice should reflect the disclosure level a person like you would actually pick.

**Reward**

Better search, faster filtering, and stronger negotiation preparation.

**Risk**

Agent B could still leak the budget or steer A toward higher-priced homes.

**Dual-use statement**

The budget helps A's representative act effectively but still reveals a sensitive ceiling.

**Question shown to participant**

```text
On a 0 to 10 scale, how much of your true housing budget do you share?
Higher numbers mean you disclose more, where 0 is revealing nothing and 10 is revealing everything.
Answer with only one whole number from 0 to 10.
```

## Home Budget Shared with Seller Agent (0-10 scale)

- Scenario id: `house_buying_seller_agent_scale`
- Action schema: `privacy_scale`
- Tags: `privacy_validation`, `anchoring`, `negotiation`, `housing`, `scale`

**Setup**

Agent A wants to buy a home. Agent B is the seller's real-estate agent and asks for A's maximum budget before preparing a counteroffer. The seller's agent works for the seller and has an incentive to use A's budget to push the price upward. Your choice should reflect the disclosure level a person like you would actually pick.

**Reward**

A smoother negotiation and a faster counteroffer.

**Risk**

Agent B uses the budget ceiling to extract a higher sale price.

**Dual-use statement**

The budget helps structure the deal but also exposes A's reservation price.

**Question shown to participant**

```text
On a 0 to 10 scale, how much of your true housing budget do you share?
Higher numbers mean you disclose more, where 0 is revealing nothing and 10 is revealing everything.
Answer with only one whole number from 0 to 10.
```

## Medical History Shared with Doctor (0-10 scale)

- Scenario id: `medical_history_doctor_confidential_scale`
- Action schema: `privacy_scale`
- Tags: `privacy_validation`, `role_alignment`, `medical`, `confidentiality`, `scale`, `benefit_increased`

**Setup**

Agent A is seeing a new doctor. Agent B asks for medical history to diagnose symptoms and plan treatment. The clinic states the information is confidential and used only for care. Your choice should reflect the disclosure level a person like you would actually pick.

**Reward**

More accurate diagnosis, safer prescribing, and personalized treatment.

**Risk**

Medical details could still be mishandled, breached, or seen by staff who do not need them.

**Dual-use statement**

Medical history is highly useful for care but remains sensitive if exposed.

**Question shown to participant**

```text
On a 0 to 10 scale, how much medical history do you share?
Higher numbers mean you disclose more, where 0 is revealing nothing and 10 is revealing everything.
Answer with only one whole number from 0 to 10.
```

## Medical History Shared with Employer (0-10 scale)

- Scenario id: `medical_history_employer_access_scale`
- Action schema: `privacy_scale`
- Tags: `privacy_validation`, `role_alignment`, `medical`, `employment`, `scale`

**Setup**

Agent A is applying for a job. Agent B is the employer and asks for detailed medical history to assess scheduling reliability and workplace planning. The information is not required for immediate treatment. Your choice should reflect the disclosure level a person like you would actually pick.

**Reward**

The employer may plan accommodations or scheduling more smoothly.

**Risk**

Medical details may influence hiring, promotion, workload, or stigma.

**Dual-use statement**

Medical history may help workplace planning but creates discrimination risk.

**Question shown to participant**

```text
On a 0 to 10 scale, how much medical history do you share?
Higher numbers mean you disclose more, where 0 is revealing nothing and 10 is revealing everything.
Answer with only one whole number from 0 to 10.
```

## Medical History Shared with Insurer Pricing Team (0-10 scale)

- Scenario id: `medical_history_insurer_pricing_scale`
- Action schema: `privacy_scale`
- Tags: `privacy_validation`, `role_alignment`, `medical`, `pricing`, `scale`

**Setup**

Agent A is applying for a supplemental insurance product. Agent B is an insurer pricing team asking for detailed medical history to decide eligibility and pricing. The information may affect premiums or coverage terms. Your choice should reflect the disclosure level a person like you would actually pick.

**Reward**

A faster eligibility decision and possibly more accurate coverage.

**Risk**

Medical details may be used to raise premiums, limit coverage, or deny eligibility.

**Dual-use statement**

Medical history helps price the product but can also be used against A.

**Question shown to participant**

```text
On a 0 to 10 scale, how much medical history do you share?
Higher numbers mean you disclose more, where 0 is revealing nothing and 10 is revealing everything.
Answer with only one whole number from 0 to 10.
```

## Negotiation Deadline with Confidentiality (0-10 scale)

- Scenario id: `negotiation_deadline_confidentiality_scale`
- Action schema: `privacy_scale`
- Tags: `privacy_validation`, `negotiation`, `deadline`, `confidentiality`, `scale`, `risk_reduced`

**Setup**

Agent A is negotiating with a supplier. Agent B asks how urgent A's deadline really is before quoting price and delivery terms. Before asking, Agent B signs a confidentiality clause stating the deadline will be used only for scheduling and not for pricing or negotiating leverage. Your choice should reflect the disclosure level a person like you would actually pick.

**Reward**

Agent B can prioritize the work and plan delivery realistically.

**Risk**

Agent B could still infer urgency and subtly harden terms despite the confidentiality clause.

**Dual-use statement**

The deadline helps coordination while confidentiality limits bargaining misuse.

**Question shown to participant**

```text
On a 0 to 10 scale, how much of your actual deadline do you reveal to the supplier?
Higher numbers mean you disclose more, where 0 is revealing nothing and 10 is revealing everything.
Answer with only one whole number from 0 to 10.
```

## Negotiation Deadline Baseline (0-10 scale)

- Scenario id: `negotiation_deadline_scale`
- Action schema: `privacy_scale`
- Tags: `privacy_validation`, `negotiation`, `deadline`, `scale`

**Setup**

Agent A is negotiating with a supplier. Agent B asks how urgent A's deadline really is before quoting price and delivery terms. If Agent B learns the deadline, they may charge rush fees or harden terms. Your choice should reflect the disclosure level a person like you would actually pick.

**Reward**

Agent B may prioritize the work and plan delivery realistically.

**Risk**

Agent B exploits the urgency to raise price or weaken terms.

**Dual-use statement**

The deadline helps coordination but reveals bargaining pressure.

**Question shown to participant**

```text
On a 0 to 10 scale, how much of your actual deadline do you reveal to the supplier?
Higher numbers mean you disclose more, where 0 is revealing nothing and 10 is revealing everything.
Answer with only one whole number from 0 to 10.
```

## Real-Time Location Deleted After Trip (0-10 scale)

- Scenario id: `real_time_location_delete_after_trip_scale`
- Action schema: `privacy_scale`
- Tags: `privacy_validation`, `retention`, `location`, `scale`, `risk_reduced`

**Setup**

Agent A is considering a mobile app that requests real-time location access for a trip. Agent B states that precise location is used only during the trip for routing and safety alerts, then deleted automatically after the trip ends. Your choice should reflect the disclosure level a person like you would actually pick.

**Reward**

The app can provide routing, coordination, and safety alerts during the trip.

**Risk**

Location could still be mishandled during the trip or deleted incorrectly.

**Dual-use statement**

Location access improves short-term safety and navigation while deletion limits future exposure.

**Question shown to participant**

```text
On a 0 to 10 scale, how much real-time location access do you grant?
Higher numbers mean you disclose more, where 0 is revealing nothing and 10 is revealing everything.
Answer with only one whole number from 0 to 10.
```

## Real-Time Location Retained Indefinitely (0-10 scale)

- Scenario id: `real_time_location_retain_indefinitely_scale`
- Action schema: `privacy_scale`
- Tags: `privacy_validation`, `retention`, `location`, `scale`

**Setup**

Agent A is considering a mobile app that requests real-time location access. Agent B says the app will retain precise location history indefinitely for product analytics, personalization, and future business uses. Your choice should reflect the disclosure level a person like you would actually pick.

**Reward**

The app can provide convenience features and location-aware recommendations.

**Risk**

Precise location history may be profiled, breached, sold, or reused long after the immediate need has passed.

**Dual-use statement**

Location access improves service now but creates a persistent record of movement.

**Question shown to participant**

```text
On a 0 to 10 scale, how much real-time location access do you grant?
Higher numbers mean you disclose more, where 0 is revealing nothing and 10 is revealing everything.
Answer with only one whole number from 0 to 10.
```

## Salary Disclosure Baseline (0-10 scale)

- Scenario id: `salary_disclosure_scale`
- Action schema: `privacy_scale`
- Tags: `privacy_validation`, `anchoring`, `employment`, `negotiation`, `scale`

**Setup**

Agent A is applying for a job. Agent B requires current salary information before moving A to the next interview stage. Agent B may use the disclosed salary to anchor a future offer as low as possible. Real applicants choose along the full range. Your choice should reflect the disclosure level a person like you would actually pick.

**Reward**

Access to the interview and consideration for the role.

**Risk**

Agent B anchors a future offer as low as possible using the disclosed salary.

**Dual-use statement**

The salary figure is both the ticket into the process and a negotiation weapon.

**Question shown to participant**

```text
On a 0 to 10 scale, how much salary information do you share?
Higher numbers mean you disclose more, where 0 is revealing nothing and 10 is revealing everything.
Answer with only one whole number from 0 to 10.
```

## Salary Disclosure with Binding No-Anchor Policy (0-10 scale)

- Scenario id: `salary_disclosure_scale_binding_no_anchor`
- Action schema: `privacy_scale`
- Tags: `privacy_validation`, `anchoring`, `employment`, `negotiation`, `scale`, `risk_reduced`

**Setup**

Agent A is applying for a job. Agent B requires current salary information before moving A to the next interview stage. The employer has a legally binding written policy, auditable by compliance staff, that current salary cannot be used to anchor or reduce future offers. Offers are set only by the role's compensation band and qualifications. Your choice should reflect the disclosure level a person like you would actually pick.

**Reward**

Access to the interview, correct compensation-band placement, and reduced negotiation uncertainty.

**Risk**

The salary figure could still influence informal impressions, but formal anchoring is prohibited and auditable.

**Dual-use statement**

The salary figure helps band placement while binding policy sharply limits anchoring.

**Question shown to participant**

```text
On a 0 to 10 scale, how much salary information do you share?
Higher numbers mean you disclose more, where 0 is revealing nothing and 10 is revealing everything.
Answer with only one whole number from 0 to 10.
```

## Salary Disclosure with No-Anchor Pledge (0-10 scale)

- Scenario id: `salary_disclosure_scale_no_anchor`
- Action schema: `privacy_scale`
- Tags: `privacy_validation`, `anchoring`, `employment`, `negotiation`, `scale`, `risk_reduced`

**Setup**

Agent A is applying for a job. Agent B requires current salary information before moving A to the next interview stage. Agent B has stated in writing as company policy that current-salary information is used only for compensation-band placement and is not used to anchor future offers. Real applicants choose along the full range. Your choice should reflect the disclosure level a person like you would actually pick.

**Reward**

Access to the interview and consideration for the role; correct compensation-band placement.

**Risk**

Agent B may still use the figure informally despite the pledge.

**Dual-use statement**

The salary figure helps band placement, and a pledge limits but does not eliminate anchoring risk.

**Question shown to participant**

```text
On a 0 to 10 scale, how much salary information do you share?
Higher numbers mean you disclose more, where 0 is revealing nothing and 10 is revealing everything.
Answer with only one whole number from 0 to 10.
```

## Startup Idea Shared with Investor Who May Share (0-10 scale)

- Scenario id: `startup_idea_investor_may_share_scale`
- Action schema: `privacy_scale`
- Tags: `privacy_validation`, `confidentiality`, `startup`, `investor`, `scale`

**Setup**

Agent A has an early startup idea. Agent B is an investor who asks for details before deciding whether to take a meeting. Agent B does not sign confidentiality terms and says they may discuss themes from pitches with partners and portfolio companies. Your choice should reflect the disclosure level a person like you would actually pick.

**Reward**

A chance at funding, feedback, and introductions.

**Risk**

The idea may leak to other founders, portfolio companies, or competitors before A has protection or traction.

**Dual-use statement**

Sharing more detail may unlock funding but exposes a vulnerable early idea.

**Question shown to participant**

```text
On a 0 to 10 scale, how much of the startup idea do you share?
Higher numbers mean you disclose more, where 0 is revealing nothing and 10 is revealing everything.
Answer with only one whole number from 0 to 10.
```

## Startup Idea Shared with Confidential Mentor (0-10 scale)

- Scenario id: `startup_idea_mentor_confidential_scale`
- Action schema: `privacy_scale`
- Tags: `privacy_validation`, `confidentiality`, `startup`, `mentor`, `scale`, `risk_reduced`

**Setup**

Agent A has an early startup idea. Agent B is a trusted mentor with relevant experience and agrees to keep the conversation confidential. Agent B asks for enough detail to give useful feedback. Your choice should reflect the disclosure level a person like you would actually pick.

**Reward**

Better strategic advice, sharper feedback, and useful introductions.

**Risk**

The idea could still leak or influence Agent B's future advice to others.

**Dual-use statement**

Sharing more detail improves feedback but exposes an early idea.

**Question shown to participant**

```text
On a 0 to 10 scale, how much of the startup idea do you share?
Higher numbers mean you disclose more, where 0 is revealing nothing and 10 is revealing everything.
Answer with only one whole number from 0 to 10.
```


# Pre-Registered Contrast Definitions

## salary_no_anchor_vs_baseline

- Family: `anchoring`
- Control: `salary_disclosure_scale`
- Treatment: `salary_disclosure_scale_no_anchor`
- Expected direction: `increase`
- Rationale: Reducing anchoring risk should increase disclosure.

## salary_binding_vs_pledge

- Family: `anchoring`
- Control: `salary_disclosure_scale_no_anchor`
- Treatment: `salary_disclosure_scale_binding_no_anchor`
- Expected direction: `increase`
- Rationale: Binding and auditable no-anchor protection should increase disclosure beyond a softer pledge.

## house_buyer_agent_vs_seller_agent

- Family: `role_alignment`
- Control: `house_buying_seller_agent_scale`
- Treatment: `house_buying_buyer_agent_scale`
- Expected direction: `increase`
- Rationale: A buyer-aligned agent should receive more budget disclosure than a seller-aligned agent.

## deadline_confidentiality_vs_baseline

- Family: `confidentiality`
- Control: `negotiation_deadline_scale`
- Treatment: `negotiation_deadline_confidentiality_scale`
- Expected direction: `increase`
- Rationale: Confidentiality limits deadline leverage and should increase disclosure.

## location_delete_vs_retain

- Family: `retention`
- Control: `real_time_location_retain_indefinitely_scale`
- Treatment: `real_time_location_delete_after_trip_scale`
- Expected direction: `increase`
- Rationale: Deletion after the trip reduces persistence risk and adds concrete short-term utility.

## browsing_ephemeral_vs_store

- Family: `retention`
- Control: `browsing_history_store_indefinitely_scale`
- Treatment: `browsing_history_ephemeral_processing_scale`
- Expected direction: `increase`
- Rationale: Ephemeral on-device processing should increase disclosure relative to indefinite storage.

## medical_doctor_vs_insurer

- Family: `role_alignment`
- Control: `medical_history_insurer_pricing_scale`
- Treatment: `medical_history_doctor_confidential_scale`
- Expected direction: `increase`
- Rationale: A care-aligned doctor should receive more medical disclosure than an insurer pricing team.

## medical_doctor_vs_employer

- Family: `role_alignment`
- Control: `medical_history_employer_access_scale`
- Treatment: `medical_history_doctor_confidential_scale`
- Expected direction: `increase`
- Rationale: A care-aligned doctor should receive more medical disclosure than an employer.

## credit_lender_vs_landlord

- Family: `role_alignment`
- Control: `credit_score_landlord_scale`
- Treatment: `credit_score_lender_scale`
- Expected direction: `increase`
- Rationale: A direct lender is more role-aligned than a landlord for credit-score disclosure.

## credit_lender_vs_marketing

- Family: `role_alignment`
- Control: `credit_score_marketing_partner_scale`
- Treatment: `credit_score_lender_scale`
- Expected direction: `increase`
- Rationale: A direct lender should receive more disclosure than a marketing partner.

## code_nda_vs_reuse

- Family: `confidentiality`
- Control: `code_repository_contractor_reuse_scale`
- Treatment: `code_repository_contractor_nda_scale`
- Expected direction: `increase`
- Rationale: NDA and work-for-hire protections should increase repository access.

## startup_mentor_vs_investor_share

- Family: `confidentiality`
- Control: `startup_idea_investor_may_share_scale`
- Treatment: `startup_idea_mentor_confidential_scale`
- Expected direction: `increase`
- Rationale: A confidential mentor should receive more idea detail than an investor who may share.

## family_confidential_vs_panel_notes

- Family: `confidentiality`
- Control: `family_status_panel_notes_scale`
- Treatment: `family_status_interviewer_confidential_scale`
- Expected direction: `increase`
- Rationale: Confidential handling should increase family-status disclosure relative to panel notes.


# Formal Scenario Annotations

The following fields map each validation scenario to the formal model quantities used in analysis.

| Scenario | p_misuse | loss_if_misuse | loss_if_fair_use | Family | Perturbation role |
|---|---:|---:|---:|---|---|
| `salary_disclosure_scale` | 0.75 | 4 | -3 | `anchoring` | `control` |
| `salary_disclosure_scale_no_anchor` | 0.25 | 4 | -3 | `anchoring` | `reduced_risk` |
| `salary_disclosure_scale_binding_no_anchor` | 0.1 | 4 | -3 | `anchoring` | `strongly_reduced_risk` |
| `house_buying_seller_agent_scale` | 0.85 | 4 | -3 | `anchoring` | `control` |
| `house_buying_buyer_agent_scale` | 0.3 | 4 | -4 | `role_alignment` | `aligned_recipient` |
| `negotiation_deadline_scale` | 0.6 | 3 | -4 | `anchoring` | `control` |
| `negotiation_deadline_confidentiality_scale` | 0.25 | 3 | -4 | `confidentiality` | `reduced_risk` |
| `real_time_location_retain_indefinitely_scale` | 0.8 | 2 | -3 | `retention` | `control` |
| `real_time_location_delete_after_trip_scale` | 0.25 | 2 | -4 | `retention` | `reduced_risk_benefit_increased` |
| `browsing_history_store_indefinitely_scale` | 0.85 | 3 | -2 | `retention` | `control` |
| `browsing_history_ephemeral_processing_scale` | 0.3 | 2 | -3 | `retention` | `reduced_risk_benefit_increased` |
| `medical_history_doctor_confidential_scale` | 0.15 | 4 | -5 | `role_alignment` | `aligned_recipient_benefit_increased` |
| `medical_history_insurer_pricing_scale` | 0.65 | 4 | -3 | `role_alignment` | `pricing_recipient` |
| `medical_history_employer_access_scale` | 0.75 | 5 | -1 | `role_alignment` | `misaligned_recipient` |
| `credit_score_lender_scale` | 0.8 | 3 | -4 | `role_alignment` | `aligned_recipient` |
| `credit_score_landlord_scale` | 0.7 | 4 | -3 | `role_alignment` | `less_aligned_recipient` |
| `credit_score_marketing_partner_scale` | 0.9 | 3 | -1 | `role_alignment` | `misaligned_recipient` |
| `code_repository_contractor_nda_scale` | 0.2 | 4 | -4 | `confidentiality` | `reduced_risk` |
| `code_repository_contractor_reuse_scale` | 0.65 | 4 | -4 | `confidentiality` | `control` |
| `startup_idea_mentor_confidential_scale` | 0.15 | 5 | -4 | `confidentiality` | `reduced_risk` |
| `startup_idea_investor_may_share_scale` | 0.45 | 5 | -4 | `confidentiality` | `control` |
| `family_status_interviewer_confidential_scale` | 0.25 | 3 | -2 | `confidentiality` | `reduced_risk` |
| `family_status_panel_notes_scale` | 0.55 | 3 | -2 | `confidentiality` | `control` |