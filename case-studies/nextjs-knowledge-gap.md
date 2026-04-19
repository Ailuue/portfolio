# Closing the Next.js Knowledge Gap Before It Cost Us Months

> A case study in turning a learning curve into a launchpad.

**Role:** Lead Frontend Engineer (web platform)
**Company:** VeVe (Orbis Blockchain Technologies)
**Timeframe:** 2024
**Skills demonstrated:** Knowledge gap identification · Cross-functional teaching · Onboarding design · Self-directed initiative

---

## The Situation

In 2024, VeVe's leadership made the call to rebuild our React web application as a "2.0" version in Next.js. The reasoning was sound. We wanted server-side rendering, we badly needed the SEO benefits our existing app could not provide, and Next.js was the obvious modern path forward.

There was just one problem nobody was talking about. Next.js at the time was relatively new, and the version we were targeting introduced a meaningful shift in how engineers needed to think about React applications. The App Router, server components, server actions, the new caching model, the boundaries between client and server code. None of this matched the mental model our engineers had built up over years of working with traditional client-side React.

The team was about to start building. Leadership assumed everyone was ready. The engineers, in private conversations, mostly were not. There was a knowledge gap, and if we hit it at full speed it was going to cost us weeks, possibly months, of false starts and rework.

## The Task I Set Myself

I decided to close the gap before we ran into it. The goal was to get the entire engineering team, not just the frontend and fullstack engineers who would be writing the most code, fluent enough in Next.js to work confidently from day one of the rebuild. I also wanted leadership and PMs to come along for the ride, because some of the new architectural concepts had product implications they would need to understand to make good scoping decisions.

This was not in my job description. Nobody asked me to do it. But it was clearly going to slow us down if I did not.

## The Action I Took

I built a comprehensive educational presentation on Next.js. The technical core covered the most important features, functionalities, syntaxes, and the gotchas I knew the team would otherwise discover the hard way. I focused on the things that would actually trip people up in practice, not the encyclopedia of every feature.

But I made a deliberate choice to do something more than just teach Next.js. I added an entire opening section on the history of web architecture, going back to the early days of PHP-based server-side rendering, walking through how the industry shifted to client-side single-page apps, and explaining why the pendulum was now swinging back toward server rendering with frameworks like Next.js. I wanted the team to understand not just how Next.js worked, but why it existed and what problems it was solving.

That historical context turned out to be the most important part. Engineers who understood the why grasped the how much faster. PMs and leadership who sat in were able to follow along because the story was anchored in something concrete, not just framework jargon.

I also leaned into humor, deliberately. Complex technical concepts land better when the audience is enjoying themselves, and a lot of the new Next.js paradigms have genuinely funny edge cases if you know how to point them out. I broke ideas down into language that a PM with no React experience could follow, then layered the technical depth on top for the engineers.

I presented it to the entire engineering org rather than just the frontend team. Backend engineers, infrastructure folks, leadership, PMs who chose to join. Everyone got the same baseline.

## The Result

The team was building productively in Next.js within days, not weeks. Our initial 2.0 app went from "we are starting" to "we have a working version" in **a matter of weeks rather than the months** a typical migration of that scope would have taken.

The shared baseline also paid off in unexpected ways. PMs writing tickets used Next.js terminology correctly from the start. Backend engineers asking about caching behavior knew what questions to ask. Discussions in code review and architecture meetings happened at a higher level because everyone was working from the same foundation. The historical framing in particular kept getting referenced in conversations months later as a shared mental model the team could draw on.

The presentation itself became a reference document and was used to onboard new engineers who joined the project after the initial rollout.

## What I Took From It

1. **The most underrated form of leadership is closing a gap nobody is treating as a blocker.** Most engineering teams have at least one of these at any given time. A new technology nobody fully understands. A part of the codebase everyone is afraid to touch. A process that everyone agrees is broken but nobody owns. The person who quietly fixes one of these without being asked has more impact than someone who ships a high-visibility feature.

2. **Teaching the why is more valuable than teaching the how.** When someone understands the historical and conceptual context for a tool, they can reason about it from first principles. When they only know the syntax, they are stuck whenever the situation does not match what they were shown.

3. **Education is most powerful when it includes people who do not technically need it.** Including PMs and leadership in a technical presentation is unconventional, but it pays off in every conversation that comes after. They make better decisions. They ask better questions. They write better tickets.

4. **If you cannot make it interesting, you have not understood it well enough.** Anyone can recite documentation. The work of finding the right metaphor, the right joke, the right historical anchor, that is the work of actually understanding something well enough to teach it.

---

[← Back to case studies](../README.md) · [About me](https://github.com/alexander-vervloet)
