## Hi, I'm Bob 👋

Founder and CEO of [BOM Quote Manufacturing](https://www.bomquote.com) and
[AsianOPS](https://www.asianops.com). I built both from the ground up and still run them day to
day with my team in Shenzhen. I also write the software they run on.

### What I run

**[BOM Quote](https://www.bomquote.com)** is global design-to-manufacturing support for hardware
teams. Design engineering, EVT/DVT, pilot and NPI builds, then production at scale out of our
Shenzhen facility. Audited by Walmart and SGS, MFi certified.

**[AsianOPS](https://www.asianops.com)** does supplier audits, quality assurance, and supply chain
engineering for medical device and pharmaceutical manufacturers sourcing from Asia. ISO 13485,
FDA QSR, GMP. Shenzhen and Hong Kong, with Orange County on the US side.

### What I'm building

**[EquatorOps](https://www.equatorops.com)**, operational change intelligence for manufacturers.
Before you approve a change to a part, a spec, a supplier, or a process, you should be able to see
everything downstream that it touches. BOMs, work orders, open POs, quality records, supplier
qualifications, inventory already in flight. Multi-tenant FastAPI and PostgreSQL, React 19 and
TypeScript, and an MCP server so an agent can query the same graph a person would.

**The AsianOPS audit platform**, which is what our auditors actually run on. It is offline first,
because a supplier audit happens on a factory floor where connectivity is not a given. Findings,
evidence photos, and CAPAs are captured locally in IndexedDB against client-generated ULIDs, then
reconciled when the auditor is back on a network. Go with chi, sqlc, and pgx behind it, React 19
and Dexie in front.

### Open source

- **[transistor](https://github.com/bomquote/transistor)** (200+ ⭐), a Python web scraping
  framework for intelligent use cases. Written in 2018 to pull electronic component pricing at
  scale for BOM Quote. Still maintained.
- **[modality](https://github.com/bomquote/modality)**, a Python framework for hardware product
  test suites. Came out of needing repeatable end-of-line testing on our own production lines.

### Why the software looks like it does

Supplier qualifications going stale. A spec revision quietly invalidating a validated process. A
BOM change landing after the POs already went out. I did not read about any of that in a
whitepaper. Every system I build is a direct answer to something that has cost my own team real
time on a real factory floor.

### Currently interested in

Multi-agent development workflows. Not the demo kind. The kind where many agents work a real
codebase in parallel with dependency tracking, file reservations, and review gates that genuinely
block a merge. It changes what a small team can hold at once.

### Stack

`Python` `FastAPI` `SQLAlchemy 2.0` `PostgreSQL` `TypeScript` `React` `Tailwind` `Astro` `Go` `C++`

### Elsewhere

[bomquote.com](https://www.bomquote.com) · [asianops.com](https://www.asianops.com) · [equatorops.com](https://www.equatorops.com)

