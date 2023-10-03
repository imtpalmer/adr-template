# DECISION

We will keep a collection of records for "architecturally significant" decisions: those that affect the structure, non-functional characteristics, dependencies, interfaces, or construction techniques.

An architecture decision record is a short text file in a format similar to an Alexandrian pattern. (Though the decisions are not necessarily patterns, they share the characteristic balancing of forces.) Each record describes a set of points and a single decision responding to those forces. Note that the decision is the central piece here, so the specific troops may appear in multiple ADRs.

We will keep ADRs in the project repository under doc/arch/ADR-NNN.md

We should use a lightweight text formatting language like Markdown or Textile.

ADRs will be numbered sequentially and monotonically. Numbers will not be reused.

If a decision is reversed, we will keep the old one around but mark it as superseded. (It's still relevant to know that it *was* the decision but is *no longer* the decision.)

We will use a format with just a few parts, so each document is easy to digest. The design has just a few features.

**Title** These documents have names that are short noun phrases. For example, "ADR 1: Deployment on Ruby on Rails 3.0.10" or "ADR 9: LDAP for Multitenant Integration."

**Context** This section describes the forces at play, including technological, political, social, and local projects. These forces are probably in tension and should be called out as such. The language in this section is value-neutral. It is simply describing facts.

**Decision** This section describes our response to these forces. It is stated in complete sentences, with an active voice. "We will …"

**Status** A decision may be "proposed" if the project stakeholders haven't agreed with it yet, or "accepted" once it is approved. If a later ADR changes or reverses a decision, it may be marked as "deprecated" or "superseded" concerning its replacement.

**Consequences** This section describes the resulting context after applying the decision. All products should be listed here, not just the "positive" ones. A particular decision may have positive, negative, and neutral consequences, but they all affect the team and project in the future.

The whole document should be one or two pages long. We will write each ADR as a conversation with a future developer. This requires a good writing style, with complete sentences organized into paragraphs. Bullets are acceptable only for visual style, not as an excuse for writing sentence fragments. (Bullets kill people, even PowerPoint bullets.)

# STATUS

Accepted.

# CONSEQUENCES

One ADR describes one significant decision for a specific project. It should affect how the rest of the project will run.

The consequences of one ADR are very likely to become the context for subsequent ADRs. This is similar to Alexander's idea of a pattern language: the large-scale responses create spaces for the smaller scale to fit into.

Developers and project stakeholders can see the ADRs, even as the team composition changes over time.

The motivation behind previous decisions is visible to everyone, present, and future. Nobody is left scratching their heads to understand, "What were they thinking?" The time to change old decisions will be clear from changes in the project's context.