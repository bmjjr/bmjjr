## Hi, I'm Bob 👋

Founder and CEO of [BOM Quote Manufacturing](https://www.bomquote.com) and
[AsianOPS](https://www.asianops.com). I built both from the ground up and still run them day to
day with my team in Shenzhen. I also write the software they run on.

### What I run

**[BOM Quote](https://www.bomquote.com)** is global design-to-manufacturing support for hardware
teams. Design engineering, EVT/DVT, pilot and NPI builds, then production at scale out of our
Shenzhen facility. Audited by Walmart and SGS, MFi certified. I wrote the customer platform behind
it and have been committing to that codebase since 2016, back when shipping software meant writing
all of it yourself.

**[AsianOPS](https://www.asianops.com)** does supplier audits, quality assurance, and supply chain
engineering for medical device and pharmaceutical manufacturers sourcing from Asia. ISO 13485,
FDA QSR, GMP. Shenzhen and Hong Kong, with Orange County on the US side.

### What I'm building

**[EquatorOps](https://www.equatorops.com)**, operational change intelligence, and a planned
spin-out of BOM Quote. Before you approve
a change to a part, a spec, a supplier, a process, or a configuration, you should be able to see
everything downstream that it touches. BOMs, work orders, open POs, quality records, supplier
qualifications, inventory already in flight.

It is built as a set of universal operational engines covering inventory, compliance, execution,
and intelligence, so one core serves aerospace and defense, construction, data centers and
infrastructure, energy and utilities, healthcare, manufacturing, regulated industries, retail and
omnichannel, SaaS platforms, field services, and warehousing and 3PL. Multi-tenant FastAPI and
PostgreSQL, React 19 and TypeScript, and an MCP server so an agent can query the same graph a
person would.

**The AsianOPS audit platform**, which is what our auditors actually run on. It is offline first,
because a supplier audit happens on a factory floor where connectivity is not a given. Findings,
evidence photos, and CAPAs are captured locally in IndexedDB against client-generated ULIDs, then
reconciled when the auditor is back on a network. Go with chi, sqlc, and pgx behind it, React 19
and Dexie in front.

### Where the idea came from

At the end of December 2018 I published
[Why you should be using model-based systems engineering in your design flow](https://www.linkedin.com/pulse/why-you-should-using-model-based-systems-engineering-your-bob/).
A late design change on a kitchen appliance had just exposed how little of a product's actual
intent is modeled anywhere. Mechanical CAD, schematics, and firmware all get built independently,
and nobody holds a model that can tell you whether they still agree. I argued that hardware teams
need a testable framework that surfaces those misalignments before manufacturing starts, not after.

I wrote **modality** that same week. EquatorOps is that argument grown up, on a much larger
surface.

### Open source

Both archived now, but they are where a lot of this started.

- **[transistor](https://github.com/bomquote/transistor)** (211 ⭐), a Python web scraping
  framework for intelligent use cases. Written in 2018 to pull electronic component pricing at
  scale for BOM Quote.
- **[modality](https://github.com/bomquote/modality)**, a Python framework for hardware product
  test suites. It matters to me well out of proportion to its star count. See above.

### Currently interested in

Multi-agent development workflows. Not the demo kind. The kind where many agents work a real
codebase in parallel with dependency tracking, file reservations, and review gates that genuinely
block a merge. It changes what a small team can hold at once.

### Stack

`Python` `FastAPI` `SQLAlchemy 2.0` `PostgreSQL` `TypeScript` `React` `Tailwind` `Astro` `Go` `C++`

### Elsewhere

[bomquote.com](https://www.bomquote.com) · [asianops.com](https://www.asianops.com) · [equatorops.com](https://www.equatorops.com)
