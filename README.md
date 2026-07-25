<div align="center">

# Bob Jordan

**Mission Viejo, CA** · Founder & CEO · Operator who writes the software

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

*I run two manufacturing companies and write the software they run on.*

![Companies founded](https://img.shields.io/static/v1?label=Companies%20founded&message=2&color=24292f&style=flat-square)
![Shipping since](https://img.shields.io/static/v1?label=Shipping%20since&message=2016&color=24292f&style=flat-square)
![Shenzhen](https://img.shields.io/static/v1?label=Floor&message=Shenzhen%20%2B%20Hong%20Kong&color=24292f&style=flat-square)
![ISO 13485](https://img.shields.io/static/v1?label=Audited%20to&message=ISO%2013485%20%C2%B7%20FDA%20QSR%20%C2%B7%20GMP&color=24292f&style=flat-square)
![MFi](https://img.shields.io/static/v1?label=Facility&message=Walmart%20%C2%B7%20SGS%20%C2%B7%20MFi&color=24292f&style=flat-square)

[![BOM Quote](https://img.shields.io/badge/bomquote.com-24292f?style=flat-square&logo=googlechrome&logoColor=white)](https://www.bomquote.com)
[![AsianOPS](https://img.shields.io/badge/asianops.com-24292f?style=flat-square&logo=googlechrome&logoColor=white)](https://www.asianops.com)
[![EquatorOps](https://img.shields.io/badge/equatorops.com-24292f?style=flat-square&logo=googlechrome&logoColor=white)](https://www.equatorops.com)
[![transistor](https://img.shields.io/badge/transistor-211%20%E2%98%85-24292f?style=flat-square&logo=python&logoColor=3776AB)](https://github.com/bomquote/transistor)

`Change Intelligence` · `Supplier Quality` · `Design-to-Manufacturing` · `MBSE` · `Offline-First Systems` · `Multi-Agent Development`

</div>

<p align="center">
<a href="#what-i-run">What I Run</a> · <a href="#what-im-building">Building Now</a> · <a href="#where-the-idea-came-from">Origin</a> · <a href="#how-i-build-now">How I Build</a> · <a href="#open-source">Open Source</a> · <a href="#connect">Connect</a>
</p>

> [!NOTE]
> I do not build operations software from a spec. I build it for two companies I own and run, one of
> which has a factory floor in Shenzhen. Every feature has a person waiting for it who I will see on
> Monday.

---

## What I Run

### [BOM Quote Manufacturing](https://www.bomquote.com)

Global design-to-manufacturing support for hardware teams. Design engineering, EVT/DVT, pilot and
NPI builds, then production at scale out of our Shenzhen facility. Injection molding, PCBA and SMT,
die casting, sheet metal. The facility is audited by Walmart and SGS, and is MFi certified.

Our customers are product design firms, high growth brands, corporate engineering teams, and
hardware entrepreneurs who need someone to carry a product from CAD to mass production without
losing the intent along the way.

I wrote the customer platform behind it and have been committing to that codebase since 2016, back
when shipping software meant writing all of it yourself.

### [AsianOPS](https://www.asianops.com)

Supplier audits, quality assurance, and supply chain engineering for medical device and
pharmaceutical manufacturers sourcing from Asia. On-site audits against ISO 13485, FDA QSR, and GMP.
Ongoing quality monitoring, technical sourcing, and program management for manufacturing
transitions.

Shenzhen and Hong Kong on one side, Orange County on the other. The credibility comes from running
our own ISO 9001 certified manufacturing facility, which means we audit suppliers as people who have
been audited.

---

## What I'm Building

### [EquatorOps](https://www.equatorops.com)

Operational change intelligence, and a planned spin-out of BOM Quote.

Before you approve a change to a part, a spec, a supplier, a process, or a configuration, you should
be able to see everything downstream that it touches. BOMs, work orders, open POs, quality records,
supplier qualifications, inventory already in flight. Most organizations discover that afterward, in
a meeting, at cost.

It is built as a set of universal operational engines covering inventory, compliance, execution, and
intelligence. One core, tenant-owned data, and eleven target industries:

`Aerospace & Defense` · `Construction` · `Data Centers & Infrastructure` · `Energy & Utilities` · `Healthcare` · `Manufacturing` · `Regulated` · `Retail & Omnichannel` · `SaaS Platforms` · `Field Services` · `Warehousing & 3PL`

Multi-tenant FastAPI and PostgreSQL with SQLAlchemy 2.0, React 19 and TypeScript on the front, an
Astro marketing surface, and an MCP server so an agent can query the same operational graph a person
would.

### The AsianOPS Audit Platform

What our auditors actually run on, and a good example of a constraint driving the architecture.

It is offline first, because a supplier audit happens on a factory floor where connectivity is not a
given and the auditor cannot stop working to wait for a network. Findings, evidence photos, and
CAPAs are captured locally in IndexedDB against client-generated ULIDs, then reconciled when the
device is back online. Photos are compressed in the browser before they ever queue.

Go with chi, sqlc, and pgx behind it. React 19, Dexie, and a PWA shell in front. Playwright across
the flows that would cost a real audit if they broke.

---

## Where the Idea Came From

At the end of December 2018 I published
**[Why you should be using model-based systems engineering in your design flow](https://www.linkedin.com/pulse/why-you-should-using-model-based-systems-engineering-your-bob/)**.

A late design change on a kitchen appliance had just exposed how little of a product's actual intent
is modeled anywhere. Mechanical CAD, schematics, and firmware all get built independently, and
nobody holds a model that can tell you whether they still agree. The mismatch surfaces during NPI,
which is the most expensive possible moment to find it. I argued that hardware teams need a testable
framework that catches those misalignments before manufacturing starts.

I wrote `modality` that same week, and spent the following year deep in SysML and Ecore tooling
trying to make the idea real.

Everything above is that argument grown up. Same problem, much larger surface, and this time with
the operational data to actually answer it.

---

## How I Build Now

Multi-agent development, at a scale that changes the work rather than decorating it.

Not the demo kind. The kind where many agents work one real codebase in parallel, with dependency
tracking across issues, advisory file reservations so two lanes cannot quietly clobber each other,
structured review gates that genuinely block a merge, and a coordination layer that keeps an audit
trail of who decided what.

The interesting problem is not getting an agent to write code. It is containment: proving that what
came back is correct, that the tests are not vacuously green, and that a lane did not widen its own
scope. A small team with good gates can hold far more surface than it used to.

---

## Open Source

Both archived now, but they are where a lot of this started.

| Project | What it is |
|---|---|
| **[transistor](https://github.com/bomquote/transistor)** · 211 ★ | A Python web scraping framework for intelligent use cases. Written in 2018 to pull electronic component pricing at scale for BOM Quote. |
| **[modality](https://github.com/bomquote/modality)** | A Python framework for hardware product test suites. It matters to me well out of proportion to its star count. See [above](#where-the-idea-came-from). |

---

## Connect

[![BOM Quote](https://img.shields.io/badge/bomquote.com-24292f?style=flat-square&logo=googlechrome&logoColor=white)](https://www.bomquote.com)
[![AsianOPS](https://img.shields.io/badge/asianops.com-24292f?style=flat-square&logo=googlechrome&logoColor=white)](https://www.asianops.com)
[![EquatorOps](https://img.shields.io/badge/equatorops.com-24292f?style=flat-square&logo=googlechrome&logoColor=white)](https://www.equatorops.com)

If you make physical things and your change process lives in spreadsheets and meetings, I would
probably enjoy talking to you.
