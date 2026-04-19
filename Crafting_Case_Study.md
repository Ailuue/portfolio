# Reframing "Crafting" From a New Section to an Integration

> A case study in how the right scope decision saves weeks.

**Role:** Lead Frontend Engineer (web platform)
**Company:** VeVe (Orbis Blockchain Technologies)
**Timeframe:** 2023
**Skills demonstrated:** Scope challenge · Technical-to-business translation · Risk-aware delivery · Architectural simplification

---

## The Situation

VeVe's product roadmap included a new feature called Crafting. The idea was elegant: let users combine multiple NFTs they already owned, "burning" them in the process, to create a new unique collectible. It was a meaningful expansion of what the platform could do, and leadership was excited about it.

The original spec proposed building Crafting as its own dedicated section of the app. New navigation. New screens. New GraphQL endpoints. A separate flow for browsing craftable items, selecting components, confirming the burn, and viewing the result. From a product vision standpoint it made sense. Crafting was a new behavior, and new behaviors often get their own home in the app.

But the more I looked at the proposed scope, the more it felt wrong. We were a lean team with a hard deadline, and we were about to build a parallel universe of UI that mirrored functionality our existing storefront already handled.

## The Task I Set Myself

I needed to make the case for a different approach without dismissing the work that had already gone into the original plan. The leaders driving this feature were not engineers, and the architectural argument I wanted to make would not land if I simply said "this is over-scoped." I needed to translate the technical reality into a business decision they could actually make.

## The Action I Took

I started by mapping the proposed Crafting flow against what already existed in our Collectible Store. The overlap was significant. Browsing, filtering, selecting items, viewing details, confirming a transaction. All of these flows existed and worked. The unique parts of Crafting were really only two things: the multi-item selection (you needed to pick the components you were burning) and the confirmation step (you needed to acknowledge that the burn was permanent).

So I proposed integrating Crafting into the existing Collectible Store rather than building a new section. Add a Craftable filter to the existing catalog. Reuse the existing item detail pages. Add a multi-select mode for the burn flow. Reuse the existing transaction confirmation pattern with a Crafting-specific warning layer.

When I presented this to leadership, I deliberately did not lead with the engineering benefits. I led with the business outcomes they cared about. Faster delivery. Less surface area for bugs. A consistent user experience where Crafting felt like a natural extension of the store rather than a separate product. The technical savings, fewer GraphQL endpoints, less duplicate frontend code, freed-up backend capacity, were the second half of the conversation, framed as "and here is why the engineering team can move faster on this."

The decision was made in that meeting. We went with the integrated approach.

The second decision I pushed for was around QA. Our team had a habit of saving QA for the end of a feature, which meant bugs surfaced late, often after the work that caused them had been forgotten. For Crafting I argued that we needed to QA continuously, after every meaningful piece of functionality landed, not just at the end. I framed this as risk reduction for the deadline. Leadership agreed, and we built QA checkpoints into the sprint plan from day one.

## The Result

We shipped Crafting **ahead of schedule.** The integration approach saved an estimated three to four weeks of frontend work and a similar amount of backend effort, allowing the team to absorb scope changes that came in late without missing the launch date.

The continuous QA approach caught dozens of bugs throughout development. Many of them were the kind that, in our usual end-loaded QA process, would have been discovered during the final week and either delayed the launch or shipped to users undetected. A handful were serious enough that finding them late could have caused a rollback.

The feature launched on time, with fewer bugs than any feature we had shipped that quarter. Users adopted Crafting quickly, in large part because it felt like a natural part of the store they already knew, not a new thing they had to learn.

## What I Took From It

1. **The instinct to give every new feature its own home is usually wrong.** New features that share core behaviors with existing ones should live alongside them. Separation creates duplicate code, duplicate UX, and duplicate maintenance, and it teaches users that your product is a collection of disconnected tools rather than a coherent experience.

2. **The way you frame a technical argument determines whether it gets heard.** Leading with business outcomes and following with technical reasoning is almost always the right order when the audience is non-technical.

3. **QA at the end is QA too late.** Building checkpoints throughout the work surfaces bugs while the context is still fresh, which is when they are cheapest to fix. This is one of those things that everyone agrees with in principle and almost no one actually does.

4. **The job of a technical voice in a product meeting is to surface the option leadership did not know they had.** The original Crafting proposal was not bad. It was just one option, and nobody else was going to suggest the alternative.

---

[← Back to case studies](../README.md) · [About me](https://github.com/alexander-vervloet)
