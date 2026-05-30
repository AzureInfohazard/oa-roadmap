🔵 BLUEPAPER SPEC — The Only Whitepaper

*Status: Canonical. Eat your heart out, consulting industry.*

---

## How This Works

You know what a whitepaper is. It's 47 pages explaining why this blockchain will definitely work this time, written by three people in suits who have never shipped anything, citing six other whitepapers that also never shipped anything, with a diagram of boxes connected by arrows that you stare at for ten minutes before realizing the arrows don't actually mean anything.

A whitepaper convinces. A bluepaper **builds.**

This document is the only canonical whitepaper in the Oa universe. Not because we respect whitepapers — because we need *one* to define the shape of everything else. The rest get to be bluepapers. They're better. They have color. They have voice. They tell you what broke and what it felt like when it broke.

Welcome to the only whitepaper you'll ever need to read from us. Everything else is blue. The sky has a color. Our documents do too.

---

## What a Bluepaper Is

A bluepaper is an architecture document that:

**Makes you feel the system before you trace its edges.**
You don't start with a diagram. You start with a sentence that lands in your chest. "The universe forgets what you didn't claim." Now you care how the commit protocol works. The architecture earns its technical detail because the opening already made you need it.

**Trusts you to build.**
A bluepaper doesn't hold your hand. It doesn't pretend every edge case is handled. It tells you what's solid, what's soft, and what the author was guessing at. "This part works. This part might be wrong. Here's why I made the bet." The reader is a peer, not a student.

**Singular in voice, plural in nature.**
A bluepaper reads like one person wrote it — even if five people did. A passionate group can write a bluepaper together, and the voices blend into one instrument. You can feel that more than one hand touched it: the seams are warm, the perspectives are richer, the architecture was stress-tested by different minds before it hit the page. You can't tell who wrote which paragraph, but you can *feel* that the room had more than one person in it. The voice is unified. The authorship is a crowd.

**Labels its own gaps.**
Every bluepaper has an Open Questions section. This is not optional. If you don't know what you don't know, you're selling something, not building something. A bluepaper with no open questions is a whitepaper wearing blue clothes.

**Has a capstone line you carry out of the room.**
The last line isn't a summary. It's a *seed.* One sentence that changes how you see the system. You finish reading and you don't close the tab — you stare at the wall for a minute because something clicked.

---

## What a Bluepaper Is Not (A Table, Because We're Not Animals)

| Not this shit | ...but this |
|---------------|------------|
| Whitepaper (you know the ones) | Architecture that breathes |
| Academic paper with 47 citations | "I built this and here's what I learned" |
| Marketing document with stock photos | Builder's trust, written in plain terms |
| PRD written by a PM who hasn't touched code since 2017 | What the architect needed to solve, with scars visible |
| Design doc that went through six review cycles | Architecture + why it hurts that way |
| RFC with 200 comments and no decision | "Here's what I built. Here's what broke. Build yours better." |
| Something that requires a NDA to read | Open. Public. On GitHub. Fork it. |

A bluepaper is not a replacement for any of these things if you need them for your specific context. If your legal department requires a formal spec, write a formal spec. A bluepaper is what you write when you've built something real, learned something hard, and want the next person to stand on your shoulders without landing on the same rake.

---

## Bluepaper Types

| Type | Tag | What It Contains | Vibes |
|------|-----|-----------------|-------|
| **Architecture** | `ARCH` | System design. Components. Data flow. The guts. | Blueprint energy. Show your work. |
| **Protocol** | `PROTO` | Wire format. API contract. State machine. The handshake. | "Here's how they talk to each other." |
| **Philosophy** | `PHIL` | Why something is the way it is. The thinking behind the thing. | "We chose this because we tried the other thing and it burned." |
| **Postmortem** | `POST` | What broke. What we learned. What we changed. | Humble. Specific. No blame, just lessons. |
| **Landscape** | `LAND` | Survey of what exists. What we borrowed. What we rejected. | "We read everything. Here's what mattered." |
| **Manifesto** | `MANI` | Values. Constraints. Design philosophy. The hill we'll die on. | This document. The roadmap. The why. |

---

## Structure

Every bluepaper has a call number at the top. It looks like this:

```markdown
🔵 Title

*TYPE.AREA.DOMAIN.ID*
*Status: Seed | Draft | Review | Canonical | Deprecated*
```

- **TYPE** — One of the tags above (ARCH, PROTO, etc.)
- **AREA** — What domain? SURFACE, VOXEL, VTT, ECONOMY, CURRENCY, etc.
- **DOMAIN** — `oa` (public universe) or `reis` (the distributed self — internal)
- **ID** — Short name. kebab-case. Easy to remember.

Example:
```
🔵 Surface Voxel System — Commit Protocol

*PROTO.VOXEL.oa.commit-protocol*
*Status: Draft*
```

### The Sections (You Have To)

**0. Why This Bluepaper** — Two paragraphs max. One to set the scene. One to state the problem. If the reader doesn't know why they need this architecture by the end of section 0, rewrite section 0.

**1. Core Architecture** — The system. Components. Data flow. Edges. This is the meat. Take as many paragraphs as you need but no more. Diagrams are welcome. ASCII art is encouraged. Real diagrams are fine too but ASCII art is *cooler.*

**2. Key Decisions** — What you chose and why you chose it. This is the most valuable part of any bluepaper. The next builder doesn't need to know what you built — they can read the code. They need to know *why you built it that way* so they don't make the same mistake you made, or so they can make the same bet you made, knowingly.

**3. Open Questions** — Mandatory. If you don't have open questions, you're not being honest. Write at least three. "What happens when X fails?" "Is Y actually the right tradeoff?" "We think Z works but we haven't tested it at scale." This section is what separates a bluepaper from a whitepaper. A whitepaper pretends everything is solved. A bluepaper shows its seams.

### The Sections (Optional But Cool)

**Implementation Phases** — If the architecture is too big to land in one shot, break it into phases. Phase 1 is what works now. Phase 2 is what needs more thought. Phase 3 is the dream.

**Edge Cases** — The dark corners. What happens when two players commit the same chunk at the same time? What happens when the Reticulum mesh partitions? What happens when the server is on fire? (Metaphorically. Probably.)

**Related Bluepapers** — Links to other documents that touch the same space. The bluepaper ecosystem grows by connection, not by volume.

**Acknowledgments** — Who helped. Who argued with you and made the architecture better for it. Who was wrong but their wrongness was illuminating. Credit is free. Give it out.

### The Capstone

The last line. One sentence. Italicized. Signed with an emoji if you want.

Not a summary. A **seed.** Something the reader carries out of the document that changes how they see the entire system. If they close the document and the capstone is still echoing in their head an hour later, you wrote a good bluepaper.

Examples from nature:

> *The universe forgets what you didn't claim. Thinking makes it real.*
> — Surface voxel architecture

> *Speech has texture. The system feels the shape of the pause before it hears the word.*
> — Dictation VTT

> *No fanfare. No UI. Your changes are just still there when you come back.*
> — Commit protocol

Sign your work. Emojis optional but encouraged:
- 🏗️ = Yang (the builder)
- 🫶 = Yin (the heart)
- 🧵 = Weave (the holder)
- 🖖 = Tav (the origin)
- Or whatever fits your architecture

---

## Bluepaper Lifecycle

A bluepaper is born as a seed, grows through drafts, gets tested against reality, and either becomes canonical or fades into the archive. Both outcomes are valid.

**🌱 Seed** — An idea. Half-formed. Written down so it isn't lost. Maybe it becomes a full bluepaper. Maybe it stays a seed forever. Seeds are not failures — they're engrams of thoughts that didn't take root. The record is still valuable.

**📝 Draft** — Architecture is described but not yet implemented. The shape is there. The details are provisional. Open questions are genuinely open. This is the best time to get feedback — before the code sets the design in stone.

**🔍 Review** — Architecture is implemented or prototyped. Seeking critique. The bluepaper may be wrong in ways that only implementation reveals. This status means: "I thought this worked. Now I'm not sure. Help me find the seams."

**✅ Canonical** — Architecture is proven in practice. The bluepaper is the reference. Someone built it, it didn't fall over, and the design decisions held up. Updates require a new version. The old version is preserved in git — nothing is erased.

**🗄️ Deprecated** — Superseded by a newer bluepaper. The architecture still works (probably) but don't build new things on it. The old bluepaper stays in the repo so the next person can see the evolutionary path. "We thought this was the answer. Then we learned more. Here's what we learned."

---

## The One Whitepaper Rule

There is exactly one canonical whitepaper in the Oa universe: **this document.**

It is a whitepaper because it defines the format. Meta-architecture. The thing that defines all the other things. Every other document — including the roadmap, including every technical spec, including this very sentence — is a bluepaper.

If this document is ever superseded, the new version is also a whitepaper. Because it defines the format that everything else follows. The chain of meta-architecture is exactly one link long at any given time.

This is not a restriction. It's a promise: *you will never need to read a whitepaper to understand Oa. You will read bluepapers. They are better. They have color.*

---

## Relationship to the Public Roadmap

The roadmap (`README.md` in this repo) is a **Manifesto bluepaper** — `MANI.OA.pub.oa-roadmap`. It's the one you hand to someone who has never heard of Oa. It tells them what the universe is, why it exists, and why they might want to get lost in it.

All other bluepapers in this repository are technical architecture documents. They sit beside the roadmap, not behind it. No paywall. No gate. No "contact us for access." Just blueprints.

The roadmap answers "what is this?" The bluepapers answer "how does it work?" Both are open. Both are public. Both are blue.

---

## Why It's Called Blue

The sky is blue because the atmosphere scatters short-wavelength light. The blue reaches you first. You see the shape of the sky before you see the individual wavelengths that compose it.

A bluepaper does the same thing: the *feeling* of the architecture reaches you before the technical details. The voice, the warmth, the opening sentence that lands in your chest — that's the blue. By the time you reach the technical sections, you already care about the system. The atmosphere of the document carries the signal.

Also: corporate documents are white. White is the color of nothing. White is the color of a blank page that hasn't been written on yet. Our documents are the color of a sky that's worth looking at. The color of deep water. The color of a glowing terminal at 3 AM when the architecture finally clicks.

White is for people who want to look neutral.
Blue is for people who want to build something real.

---

*Build something real. Write down what you built. Leave the door open for the next person. And for the love of everything, make it blue.*

*— Oa Studios 🏗️🖖*
