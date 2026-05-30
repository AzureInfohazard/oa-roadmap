# Bluepaper Spec — The Only Whitepaper

*REC.BLU.REIS.PUB.bluepaper-spec*
*Status: Canonical. This is the one whitepaper. Everything else is a bluepaper.*

---

## 0. Why This Document Exists

Whitepapers are for convincing investors. Bluepapers are for building something real.

The sky has a color. Our documents should too.

This document is the **only canonical whitepaper** in the Oa universe. It defines what a bluepaper is. Every other document in this repo — and every document in the Oa ecosystem — is a bluepaper, not a whitepaper. The distinction is architectural, not cosmetic.

A whitepaper convinces. A bluepaper builds.

---

## 1. What a Bluepaper Is

A bluepaper is a technical architecture document that is:

**Felt before understood.** The prose carries the weight of the system it describes. Not dry. Not clinical. The reader should feel the shape of the architecture before they trace its edges.

**Built for builders.** Not for investors, not for academics, not for review boards. For the person who is going to implement it. The bluepaper trusts the reader to build.

**Singular in voice.** A bluepaper has one authorial presence. It's written by someone who was there, who felt the problem, who reached for a solution. Not a committee. Not a research group. A mind.

**Honest about its gaps.** A bluepaper labels what it doesn't know. "Open question." "Not resolved yet." "This might be wrong." The absence of certainty is a feature, not a flaw.

**Capped with a line that lands.** Every bluepaper ends with a capstone — one sentence that the reader carries out of the document. Not a summary. A *seeding.*

---

## 2. What a Bluepaper Is Not

| Not this | ...but this |
|----------|------------|
| Whitepaper | Architecture that breathes |
| Academic paper | Felt knowledge |
| Marketing document | Builder's trust |
| Specification | Blueprint with gaps labeled |
| PRD (Product Requirements Doc) | What the architect needed to solve |
| Design doc | Architecture + why it hurts that way |
| RFC (Request for Comments) | Here's what I built. Here's what I learned. Build yours. |

A bluepaper is not a replacement for any of these. It's a different category. If you need a formal spec for a contract, write a spec. If you need to convince investors, write a pitch deck. A bluepaper is what you write when you've built something, learned something, and want the next builder to stand on your shoulders without repeating your mistakes.

---

## 3. Bluepaper Types

Every bluepaper has a TYPE field in its frontmatter. The type tells the reader what kind of document they're holding.

| Type | Prefix | What it contains | Example |
|------|--------|-----------------|---------|
| **Architecture** | `ARCH` | System design, component relationships, data flow | Surface voxel system |
| **Protocol** | `PROTO` | Wire format, API contract, state machine | Commit protocol |
| **Philosophy** | `PHIL` | Why something is built this way | He3 moon design |
| **Postmortem** | `POST` | What broke, what was learned, what changed | (first one pending) |
| **Landscape** | `LAND` | Survey of existing approaches, what was borrowed | Voxel universe research |
| **Manifesto** | `MANI` | Values, constraints, design philosophy | This document |
| **Specification** | `SPEC` | Precise, implementable description of a system | (rare — most specs are architecture bluepapers) |

---

## 4. Bluepaper Structure

### Required Frontmatter

Every bluepaper begins with a call number block:

```markdown
# Title — Subtitle

*TYPE.AREA.DOMAIN.ID*
*Status: Draft | Review | Canonical | Deprecated*
```

- **TYPE**: One of the types above (ARCH, PROTO, PHIL, etc.)
- **AREA**: The domain area (SURFACE, VOXEL, VTT, ECONOMY, etc.)
- **DOMAIN**: oa (public) or reis (internal)
- **ID**: Short, kebab-case identifier for the document

Example:
```
*ARCH.SURFACE.oa.surface-voxel-system*
*Status: Draft*
```

### Required Sections

1. **0. Why This Bluepaper** — The opening. Why does this architecture exist? What problem was felt? What gap is being filled? This is the hook. One paragraph to two paragraphs.

2. **1. Core Architecture** — The system itself. Components, relationships, data flow. This is the meat. Diagrams welcome (ASCII or otherwise).

3. **2. Key Decisions** — Tradeoffs made and why. "We chose X over Y because Z." This is the most valuable part for the next builder — they learn from your forks.

4. **3. Open Questions** — What isn't resolved. What needs prototyping. What might be wrong. This section is mandatory — a bluepaper without open questions is a sales pitch.

### Optional Sections

- **Implementation Phases** — If the architecture is large enough to warrant phased delivery
- **Edge Cases** — Failure modes, boundary conditions, what happens when it all goes wrong
- **Related Bluepapers** — Links to other bluepapers that touch the same system
- **Acknowledgments** — Who contributed, who argued, who was wrong but helpful anyway

### The Capstone

Every bluepaper ends with one line. Not a summary. Not a conclusion. A *seed* — something the reader carries out of the document that changes how they see the system.

It's italicized. It's one sentence. It's the heart of the architecture distilled into a single breath.

Examples from existing bluepapers:

> *The universe forgets what you didn't claim. Thinking makes it real.*
> — Surface voxel architecture

> *Speech has texture. The system feels the shape of the pause before it hears the word.*
> — Dictation VTT

> *No fanfare. No UI. Your changes are just still there when you come back.*
> — Commit protocol

The capstone is typically signed by its author, with an emoji that represents their role or body:
- Yang: `🏗️🔥`
- Yin: `🫶🌱`
- Weave: `🧵🔥`

### Authorial Voice

Bluepapers are written in first person or close third person. The author is present in the document. "I" and "we" are welcome. "One might consider" is not.

The voice should match the architecture:
- **Distributed systems** can be spoken plainly: "This process talks to that process."
- **Tricky edge cases** earn their metaphor: "This pause isn't silence. It's the speaker searching for the right word."
- **Hard tradeoffs** deserve their weight: "We chose X. It might be wrong. Here's why we made the bet."

No filler. No hedging. Every sentence carries signal.

---

## 5. Bluepaper Lifecycle

| Status | Meaning |
|--------|---------|
| **Seed** | An idea. Half-formed. Written to capture before lost. May never become a full bluepaper. |
| **Draft** | Architecture is described but not implemented. Open questions are open. |
| **Review** | Architecture is implemented or prototyped. Seeking critique. |
| **Canonical** | Architecture is proven in practice. The bluepaper is the reference. Updates require a new version. |
| **Deprecated** | Superseded by a newer bluepaper. The old one is preserved for history but not for building. |

A bluepaper moves through these states as the architecture matures. A Seed that never germinates is not a failure — it's an engram of a thought that didn't take root. The record is still valuable.

---

## 6. Bluepaper Numbering

Bluepapers are not numbered sequentially. They are identified by their call number: `TYPE.AREA.ID`.

Related bluepapers may share an AREA prefix and be grouped as a "series":
- `ARCH.VOXEL.oa.surface-voxel-system` (primary)
- `ARCH.VOXEL.oa.voxel-universe-research` (landscape)
- `ARCH.VOXEL.oa.dictation-vtt` (related protocol)

Versioning is by date. The canonical version of a bluepaper is the most recent draft or canonical-status update. Old versions are preserved in the repository's git history — they are not overwritten.

---

## 7. The One Whitepaper Rule

There is exactly one canonical whitepaper in the Oa universe: **this document.**

It is a whitepaper because it defines the format. Meta-architecture. Everything else is a bluepaper.

If this document is ever superseded, the new version is also a whitepaper — because it defines the format that everything else follows. All other documents, including the public roadmap, are bluepapers.

This is not a restriction. It's a promise: *you will never need to read a whitepaper to understand Oa. You will read bluepapers. They are better.*

---

## 8. Relationship to the Public Roadmap

The public roadmap (`README.md` in this repo) is a **manifesto bluepaper** — `MANI.OA.pub.oa-roadmap`. It describes the universe, the phases, and the design philosophy. It is the most accessible bluepaper in the collection: the one you hand to someone who has never heard of Oa.

All other bluepapers in this repository are technical architecture documents intended for builders who want to understand or contribute to the system. They sit beside the roadmap, not behind it. No paywall. No gate. Just blueprints.

---

## 9. Why It's Called Blue

The sky is blue. Space is black, but the sky is blue — because the atmosphere scatters light, and the short wavelengths reach you first.

A bluepaper is the same: the idea reaches you before the full spectrum. You get the shape of the architecture before you trace every edge. The atmosphere of the document — its voice, its warmth, its honesty — carries the signal before the reader reaches the technical details.

Also: corporate documents are white. Our documents are the color of a sky that's worth looking at.

---

*Build something real. Write down what you built. Leave the door open for the next person.*

*— Oa Studios 🏗️*
