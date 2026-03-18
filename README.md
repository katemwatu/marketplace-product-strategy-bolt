# marketplace-product-strategy-bolt
# Marketplace Product Strategy — Bolt

Two-part Senior PM submission for Bolt, the European ride-hailing platform 
operating across 45+ countries. Covers both proactive feature strategy and 
reactive data-driven problem solving — two core PM modes in one document.

---

## Part 1: Scheduled Rides — Feature Strategy

### The Strategic Question
Bolt's on-demand model creates anxiety for time-sensitive trips (airports,hospital appointments). The question isn't whether to build scheduling — it's whether Bolt can solve the underlying marketplace constraint 
(driver supply) well enough to make the feature trustworthy.

> *"Success is contingent on solving the core marketplace constraint of 
> driver supply, not just building a rider-facing UI."*

### Dual-Sided Problem Framing

| Side | Pain Point | Opportunity |
|---|---|---|
| Riders | No reliability guarantee for critical trips → churn to competitors | Premium-priced certainty; improved 30-day retention |
| Drivers | Inconsistent demand → unpredictable earnings | Predictable, pre-planned high-value trips |

### Solution Design Highlights
- **Locked-in pricing**: Standard Fare + 10% scheduling premium — simple,defensible, incentivises driver acceptance
- **Fallback mechanism**: If no driver accepts 60 minutes before pickup, system auto-initiates on-demand matching — protects the promise without overpromising
- **Driver autonomy**: Opt-in toggle, earnings preview dashboard, priority access to high-value trips for reliable drivers
- **Acceptance criteria written for both sides**: 
  separate S/R/D criteria for System, Rider, and Driver flows

### Phased Rollout (Risk-First)

| Phase | Duration | Goal |
|---|---|---|
| 1 — Proof of Concept | 4–6 weeks | Validate UX flows, finalise pricing algorithm |
| 2 — Alpha (Bolt employees) | 4 weeks | End-to-end operational stack test |
| 3 — City Beta | 8 weeks | Achieve >98% fulfillment rate before expansion |
| 4 — Regional Expansion | Ongoing | Scorecard-gated city-by-city rollout |
| 5 — Feature Expansion | Post-beta | Recurring rides for commuters |

### Success Metrics

| Metric | Target |
|---|---|
| Scheduled ride adoption | >5% of active users in 3 months |
| Fulfillment rate | >95% on-time within 5 minutes |
| Driver acceptance rate | >90% of scheduled requests |
| 30-day repeat scheduling | >40% |
| Incremental GMV | +0.5% |
| Rider NPS vs. regular rides | +15 points |

---

## Part 2: Overcharge Ticket Reduction — Data Analysis

### The Problem
337 overcharge support tickets analysed. Three root causes identified:

| Issue | Ticket Count | % of Total |
|---|---|---|
| Missing upfront pricing | 229 | 68% |
| Low GPS confidence | 201 | 60% |
| High price deviation from prediction | 77 | 23% |

*Note: Issues overlap — a single ticket can exhibit multiple factors.*

### Root Cause Insights
- **Missing upfront price** is the dominant driver: riders without a reference price form expectations based on past trips. Any mismatch feels like overcharging — even when pricing is technically correct
- **GPS confidence** is an operational amplifier: 3 in 5 overcharge 
  tickets occur during low GPS confidence periods, particularly in 
  rural or signal-poor environments
- **Prediction model drift**: when the upfront quote doesn't account for real-time traffic or route deviations, even price-informed ridersexperience shock at checkout

### Remediation Roadmap

| Timeframe | Actions | Expected Outcome |
|---|---|---|
| 0–3 months | 15% price cap on predicted fares; automated partial refunds; proactive GPS confidence warnings | Immediate reduction in price shock |
| 3–6 months | Manual pin-drop for low-confidence pickups; updated fare estimates after destination changes | Fewer inaccurate routes, improved trust |
| 6–12 months | Rebuild prediction model with real-time contextual variables; retrain on local data | Structural 40–50% reduction in overcharge tickets |

### Target Outcome
> 40–50% reduction in overcharge tickets within 6 months — 
> restoring rider trust and reducing support costs.

---

## What This Demonstrates

- **Dual-sided marketplace thinking**: solutions designed for both 
  supply and demand simultaneously
- **Hypothesis-driven analysis**: overcharge investigation started with 5 explicit hypotheses before touching the data
- **Risk-first rollout design**: phased launch gated on fulfillment 
  rate, not calendar date
- **Proactive vs. reactive PM modes**: Part 1 is strategic/forward-looking; 
 Part 2 is analytical/diagnostic — both in one submission
- **UX depth**: separate rider and driver journeys with specific 
  acceptance criteria per user type

## Deliverable
[View the full submission (PDF)](./PM_Hometask.pdf)

---

*Applied as part of a Senior PM interview process.*
*The financial modelling in this submission was subsequently strengthened — 
see [B2B SaaS Feature Strategy – Smart Rotations](../b2b-saas-feature-strategy-smart-rotations) 
for the evolved approach.*
