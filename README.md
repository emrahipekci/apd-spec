# APD — Autonomous Project Delivery Protocol

A formal multi-agent coordination protocol for adversarial multi-stakeholder project delivery and operations.

## What is APD?

APD is a domain-specific application-layer protocol that enables autonomous software agents to coordinate project delivery across organisational boundaries — where participants have independent mandates, competing interests, and legally binding obligations.

Unlike cooperative multi-agent frameworks that assume shared goals, APD is designed for the real world: an owner’s agent protects the owner’s interests, a contractor’s agent protects the contractor’s interests, and the protocol ensures coordination without requiring trust.

**Seven integrated specifications:**

1. **Ecosystem Model** P=(E,R,C) — every entity, relationship, and constraint
1. **Role Virtualisation** V:H→A — mapping human roles to agent configurations
1. **Authority Matrix** AM — three-tier decision governance (autonomous, consensus, human-in-the-loop)
1. **Communication Model** — six-function taxonomy with authority-governed routing
1. **Workflow Engine** — HITL-gated finite state machines with contractual time constraints
1. **Contract Rules Engine** — five-stage pipeline converting governing instruments into machine-executable obligations
1. **Project State Vector** PS(t) — continuous, immutable, causally linked record of every action and decision

The protocol is **domain-agnostic by design, domain-specific by configuration**. The same seven specifications can govern a house renovation, a $1.2B power plant, a pharmaceutical development programme, or a million-contributor open science collaboration. The configuration changes. The protocol does not.

## Current Status

APD is a **design-only specification** as of April 2026. The specification is complete and published. Implementation and validation are next.

## Paper

**“Autonomous Project Delivery: A Formal Multi-Agent Coordination Protocol for Adversarial Multi-Stakeholder Environments”**

Emrah Ipekci (2026)

- **SSRN:** <https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6487399>
- **arXiv:** Submission pending (cs.MA)

Seven formal specifications, complete reference configuration with evaluation metrics.

## Protocol Stack Position

```
Transport (HTTP / gRPC / JSON-RPC 2.0)
    └── MCP (Model Context Protocol) — agent-to-tool
        └── A2A (Agent-to-Agent Protocol) — peer-to-peer
            └── APD (this protocol) — domain-specific coordination
```

APD operates above MCP and A2A, adding identity, authority, contractual semantics, and coordination governance that infrastructure protocols do not provide.

## Key Concepts

**Adversarial coordination:** Participants are independently mandated parties with competing interests — not teammates with a shared goal. APD coordinates despite conflicting interests, not by assuming they don’t exist.

**Governing instruments:** APD governs against contracts, regulations, laws, standards, permits, insurance policies, and any other obligation-creating instrument — not just “contracts.”

**Graduated autonomy:** Five maturity levels from AI-assisted human coordination (Level 1, deployable today) through fully autonomous delivery (Level 4). Human oversight is a permanent design principle.

**Progressive elaboration:** APD does not require complete setup to begin. The protocol grows with the project as new information, new parties, and new work packages emerge.

## Repository Structure

```
apd-spec/
├── README.md           ← you are here
├── paper/              ← specification paper
├── examples/           ← domain configuration examples
│   ├── house-build/    ← residential construction walkthrough
│   ├── software-dev/   ← software development configuration
│   └── open-science/   ← scientific collaboration configuration
└── schema/             ← machine-readable configuration schemas (planned)
```

## Related Repositories

- [`deeptask`](https://github.com/apd-protocol/deeptask) — APD’s first empirical validation experiment: a task management app built by AI agents under cooperative vs APD-governed coordination
- `apd-core` — minimal APD protocol library (planned)
- `apd-examples` — community configuration examples (planned)

## How to Contribute

APD is an open protocol. Contributions are welcome:

- **Researchers:** Review the specification, identify gaps, propose extensions
- **Developers:** Build implementations on MCP+A2A infrastructure
- **Practitioners:** Share domain configurations (construction, software, manufacturing, healthcare, etc.)
- **Domain experts:** Validate the protocol against your industry’s coordination challenges

Open an issue to start a discussion, or reach out directly.

## About the Author

**Emrah Ipekci** — Chartered Civil Engineer (CEng), MSc, MBA, PMP. 20+ years directing combined-cycle gas turbine (CCGT) megaprojects across Turkey, Russia and Uzbekistan. The practitioner who needed the protocol that multi-agent systems research had not yet built.

- **ORCID:** [0009-0008-0328-8245](https://orcid.org/0009-0008-0328-8245)
- **SSRN:** [Emrah Ipekci](https://papers.ssrn.com/sol3/cf_dev/AbsByAuth.cfm?per_id=7610498)
- **Email:** [to be added]

## Citation

```bibtex
@article{ipekci2026apd,
  title={Autonomous Project Delivery: A Formal Multi-Agent Coordination Protocol 
         for Adversarial Multi-Stakeholder Environments},
  author={Ipekci, Emrah},
  journal={SSRN Electronic Journal},
  year={2026},
  note={SSRN 6487399}
}
```

## License

- **Protocol specification:** © 2026 Emrah Ipekci. All rights reserved. Patent pending.
- **Code in this repository:** MIT License
- **Configuration examples:** CC-BY 4.0

-----

*APD is domain-agnostic by design, domain-specific by configuration. Your project is a configuration. The protocol is the same.*
