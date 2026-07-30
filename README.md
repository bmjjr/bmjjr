<div align="center">

# Bob Jordan

**Mission Viejo, CA** · CEO & Chief Architect · [EquatorOps](https://www.equatorops.com) · [BOM Quote](https://www.bomquote.com) · [AsianOPS](https://www.asianops.com)

![Python](https://img.shields.io/badge/-Python-24292f?style=flat-square&logo=python&logoColor=3776AB)
![TypeScript](https://img.shields.io/badge/-TypeScript-24292f?style=flat-square&logo=typescript&logoColor=3178C6)
![Go](https://img.shields.io/badge/-Go-24292f?style=flat-square&logo=go&logoColor=00ADD8)
![FastAPI](https://img.shields.io/badge/-FastAPI-24292f?style=flat-square&logo=fastapi&logoColor=009688)
![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-24292f?style=flat-square&logo=postgresql&logoColor=4169E1)
![React](https://img.shields.io/badge/-React-24292f?style=flat-square&logo=react&logoColor=61DAFB)
![Tailwind](https://img.shields.io/badge/-Tailwind-24292f?style=flat-square&logo=tailwindcss&logoColor=06B6D4)
![Astro](https://img.shields.io/badge/-Astro-24292f?style=flat-square&logo=astro&logoColor=FF5D01)
![C++](https://img.shields.io/badge/-C++-24292f?style=flat-square&logo=cplusplus&logoColor=00599C)
![Claude](https://img.shields.io/badge/-Claude-24292f?style=flat-square&logo=anthropic&logoColor=d4a27f)

*Turning organizational knowledge into computable change impact.*

![Companies founded](https://img.shields.io/static/v1?label=Companies%20founded&message=3&color=24292f&style=flat-square)
![Years in manufacturing](https://img.shields.io/static/v1?label=In%20manufacturing&message=25%2B%20years&color=24292f&style=flat-square)
![Units shipped](https://img.shields.io/static/v1?label=Client%20units%20shipped&message=1M%2B&color=24292f&style=flat-square)
![Retail value](https://img.shields.io/static/v1?label=Retail%20sales%20value&message=%24100M%2B&color=24292f&style=flat-square)
![Certifications](https://img.shields.io/static/v1?label=Operating%20to&message=ISO%209001%20%C2%B7%20ISO%2013485%20%C2%B7%20FDA%20QSR&color=24292f&style=flat-square)

[![EquatorOps](https://img.shields.io/badge/equatorops.com-24292f?style=flat-square&logo=googlechrome&logoColor=white)](https://www.equatorops.com)
[![BOM Quote](https://img.shields.io/badge/bomquote.com-24292f?style=flat-square&logo=googlechrome&logoColor=white)](https://www.bomquote.com)
[![AsianOPS](https://img.shields.io/badge/asianops.com-24292f?style=flat-square&logo=googlechrome&logoColor=white)](https://www.asianops.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square)](https://www.linkedin.com/in/bjordan1/)
[![transistor](https://img.shields.io/badge/transistor-211%20%E2%98%85-24292f?style=flat-square&logo=python&logoColor=3776AB)](https://github.com/bomquote/transistor)

`Change Intelligence` · `Scenario Simulation` · `Signal-to-Action` · `Supplier Quality` · `Design-to-Manufacturing` · `MBSE` · `Offline-First Systems` · `Multi-Agent Development`

</div>

<p align="center">
<a href="#equatorops">EquatorOps</a> · <a href="#the-operating-companies">Operating Companies</a> · <a href="#where-the-change-intelligence-focus-came-from">Origin</a> · <a href="#the-software-factory">Software Factory</a> · <a href="#open-source">Open Source</a> · <a href="#before-all-this">Background</a> · <a href="#connect">Connect</a>
</p>

> [!NOTE]
> I founded and operate three companies: design-to-manufacturing, supply chain and QA engineering
> consulting, and operational change intelligence. BOM Quote and AsianOPS run on EquatorOps today.
> Client Zero is my own company, and the platform gets validated against real operational complexity
> every day rather than against a roadmap.

---

## EquatorOps

**[equatorops.com](https://www.equatorops.com)** · CEO & Chief Architect · codebase started 2019

Most operational software records work after the fact. EquatorOps answers the question that actually
costs money: if we make this change, what breaks?

Too often that answer lives in tribal knowledge. One experienced person knows which work orders will
slip. Someone else knows which approvals are required, which documents need revision, which
suppliers are affected, or which evidence has to be re-run. That knowledge is fragile, expensive,
and no one holds all of it at once.

The **Verification Graph Engine** models the organization as one graph across the silos that
normally cannot see each other: parts and BOMs, suppliers, inventory, work orders, documents,
approvals, evidence, and the change record itself. The relationships are not hand-drawn. Each domain
contributes its own from the records it already owns, so the graph reflects the current state of the
business rather than a parallel model somebody has to maintain. Changes and operational signals run
against it to compute consequences: what a signal touches, what it may delay or invalidate, what
evidence has to be re-established, what needs approval, who has to act, and what should move first.

**Impact Intelligence** turns that into a decision. A change you have not made yet is a first-class
object. A signal arrives, whether that is a supplier going on hold, a revised specification, a
failed test, or a shipment that will not land in time. You open a case against it, write down the
alternatives, and the system compiles each one into a proposed graph and runs them against a single
identical snapshot of the business taken at one instant. You compare, select, and the winner becomes
a Draft Change Control exactly once, with nothing retyped and no second copy under a retry. No
system of record is touched to find out what touching it would do.

Two things make the simulation trustworthy. It models what a change removes, not only what it adds,
and a relationship disappears only when the change takes away its last remaining cause: a document
that three regulations require does not stop being required when one of them is withdrawn. And it is
contained by construction: proposed runs are marked on every edge and cannot be signed, packed into
an evidence bundle, exported, or reused as a real result, which is what makes it safe to run
hypotheticals inside a system whose other output is audit evidence. Cases, baselines, runs, and
decisions are immutable and lineage linked, so months later you can still answer what was known at
the time, what the system said, who chose, and whether the change did what it promised once it
shipped.

It scales past one decision. Findings normalize across cases, so a recurring consequence stops being
rediscovered by hand every time. Batches evaluate many proposed changes together and rank what moves
first. Signals arrive from connected systems and field observations rather than only from a person
noticing. And because the whole surface is an API with an MCP server in front of it, an agent
queries the same operational graph, under the same authority and the same refusals, that a person
would.

Underneath it: programmable operational engines for BOMs, inventory, assets, purchasing, work
orders, quality, compliance, documents, and change control, delivered as tenant-scoped APIs. I
architected the 370+ table schema, the 70+ API surfaces, and the event-driven backend.

`Manufacturing` · `Regulated & Life Sciences` · `Aerospace & Defense` · `Energy & Utilities` · `Construction` · `Data Centers & Infrastructure` · `Field Services` · `Warehousing & 3PL`

Multi-tenant FastAPI and PostgreSQL with SQLAlchemy 2.0, React 19 and TypeScript on the front, and an
Astro marketing surface.

---

## The Operating Companies

### [BOM Quote Manufacturing](https://www.bomquote.com) · founded 2011

End-to-end product design and contract manufacturing for complex electromechanical programs. Design
engineering, EVT/DVT, pilot and NPI builds, then production at scale out of our Shenzhen facility.
Injection molding, PCBA and SMT, die casting, sheet metal.

Over time BOM Quote has helped ship more than **1M units representing over $100M in retail sales
value**, including programs placed in Best Buy, Target, and Walmart. ISO 9001 certified and approved
under Walmart Responsible Sourcing. We also designed, manufactured, and launched our own
direct-to-consumer line, HoneyGear.

I wrote the customer platform behind it and have been committing to that codebase since 2016, back
when shipping software meant writing all of it yourself.

### [AsianOPS](https://www.asianops.com) · founded 2010

A boutique operations and supply chain consultancy helping Western companies build, de-risk, and
manage manufacturing and technical operations in China. On-the-ground engineering, sourcing,
supplier development, quality control, compliance, and execution management.

The work spans consumer electronics, electromechanical products, and Class II and III medical device
programs, audited against ISO 13485, FDA QSR, and GMP. Shenzhen and Hong Kong on one side, Orange
County on the other.

The firm's role has consistently been to close the gap between what companies plan and what actually
happens across factories, suppliers, labs, documents, approvals, and handoffs. That gap is the
entire reason EquatorOps exists.

### The AsianOPS Audit Platform

What our auditors actually run on, and a good example of a constraint driving the architecture.

It is offline first, because a supplier audit happens on a factory floor where connectivity is not a
given and the auditor cannot stop working to wait for a network. Findings, evidence photos, and
CAPAs are captured locally in IndexedDB against client-generated ULIDs, then reconciled when the
device is back online. Photos are compressed in the browser before they ever queue.

Go with chi, sqlc, and pgx behind it. React 19, Dexie, and a PWA shell in front. Playwright across
the flows that would cost a real audit if they broke.

---

## Where the Change Intelligence Focus Came From

At the end of December 2018 I published
**[Why you should be using model-based systems engineering in your design flow](https://www.linkedin.com/pulse/why-you-should-using-model-based-systems-engineering-your-bob/)**.

A late design change on a kitchen appliance had just exposed how little of a product's actual intent
is modeled anywhere. Mechanical CAD, schematics, and firmware all get built independently, and
nobody holds a model that can tell you whether they still agree. The mismatch surfaces during NPI,
which is the most expensive possible moment to find it. I argued that hardware teams need a testable
framework that catches those misalignments before manufacturing starts.

I wrote `modality` that same week, and spent the following year deep in SysML and Ecore tooling
trying to make the idea real. I started the EquatorOps codebase the year after that.

Same problem, much larger surface, and this time with the operational data to actually answer it.

---

## The Software Factory

We designed and built our own software factory for multi-agent swarm development. It runs on the
EquatorOps Agent Coordination API, so the swarm coordinates through the same platform we sell.

**The protocol is the interop layer.** A lane is not bound to a vendor. An Anthropic implementer and
an OpenAI reviewer coordinate cleanly on the same run, because what they share is a typed message
contract, a canonical thread, and a lease, not a common SDK. Any model that can hold a shell and
speak the contract can take a lane, including open-weight and Chinese models. Provider is a recorded
field, never an assumption baked into the tooling.

| Role | Responsibility |
|---|---|
| **Implementer** | Owns a lane, holds file reservations, submits for review. |
| **Reviewer** | Claims review requests under an atomic lease. Runs as a deterministic daemon that invokes a model only when a review is claimed, so nothing idles burning tokens. |
| **Run-manager** | One per run. Preflights, launches, monitors lane health, triages stuck lanes, gates phase transitions. |

Runs are declared as **workorders** and gated before any agent launches: manifest lint, a Definition
of Ready check, and layered validation including live API integration. Launch identity is computed
into a plan artifact rather than derived by convention, so every participant resolves the same
session, threads, and announcer.

The mechanisms that make it hold:

- **Exclusive file reservations** with TTL. Any file two teams touch requires one, which is what
  stops parallel lanes silently clobbering each other.
- **Review as a protocol.** An approved verdict is rejected without pre-commit evidence attached.
  The requester then files adoption and resolution ledger entries naming which findings were taken
  and which were deferred, and the server enforces provenance against the canonical review lineage.
  A lane cannot manufacture its own sign-off.
- **Closeout as a state machine**, not a claim: `review_cleared_closeout_ready` →
  `canonical_artifacts_present` → `acceptance_pending` → `session_complete`. Artifacts carrying the
  wrong session ref, wrong team, or broken lineage are ignored rather than counted.
- **A supervised run-manager.** A watcher classifies provider failures from pane evidence, nudges
  transient faults with bounded backoff, and restarts genuine exits from recorded launch identity.
  Liveness resolves by walking process descendants, so a provider running as a native grandchild
  under a launcher thread reads as alive. Recovery state persists atomically across the watcher's
  own crash, and a quota ladder fails over across providers rather than retrying into a rate limit.

The interesting problem was never getting an agent to write code. It is containment: proving what
came back is correct, that the tests are not vacuously green, and that a lane did not quietly widen
its own scope.

There is an obvious symmetry between that and the day job. Both are about knowing what a change
actually touches before you let it through, and both come down to the same rule: a lane cannot
manufacture its own sign-off, and a hypothetical run cannot manufacture evidence.

---

## Open Source

Both archived now, but they are where a lot of this started.

| Project | What it is |
|---|---|
| **[transistor](https://github.com/bomquote/transistor)** · 211 ★ | A Python web scraping framework for intelligent use cases. Written in 2018 to pull electronic component pricing at scale for BOM Quote. |
| **[modality](https://github.com/bomquote/modality)** | A Python framework for hardware product test suites. It matters to me well out of proportion to its star count. See [above](#where-the-change-intelligence-focus-came-from). |

---

## Before All This

I did not start in software.

Seven years as a chemical operator at BASF, working full time while finishing my degree. Then shop
floor operations at Guardian Industries, leading 100+ people across production, quality, and
shipping. Then a greenfield startup team at Cardinal Glass, where I built a manufacturing department
from nothing, hired 60+ people across three shifts, and helped take the facility from $0 to $20M in
sales in two years.

An MBA at UVA Darden, supply chain consulting at PRTM, then running the outsourcing of a Class II
medical device program from California to China for Tria Beauty, which took 40% out of COGS in a
year.

Twenty five years of that operational exposure is what pointed me at change intelligence. I have
spent a lot of my career being the person who finds out about an undesired change impact too late,
and I know how much value is sitting in that gap. The knowledge required to catch it almost always
exists somewhere in the organization already. It just lives in someone's head, which is exactly why
the work now is turning organizational knowledge into computable change impact.

---

## Connect

[![EquatorOps](https://img.shields.io/badge/equatorops.com-24292f?style=flat-square&logo=googlechrome&logoColor=white)](https://www.equatorops.com)
[![BOM Quote](https://img.shields.io/badge/bomquote.com-24292f?style=flat-square&logo=googlechrome&logoColor=white)](https://www.bomquote.com)
[![AsianOPS](https://img.shields.io/badge/asianops.com-24292f?style=flat-square&logo=googlechrome&logoColor=white)](https://www.asianops.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square)](https://www.linkedin.com/in/bjordan1/)

If your change process lives in spreadsheets, tribal knowledge, and meetings, I would probably enjoy
talking to you.
