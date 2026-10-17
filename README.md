![Agent Co-op](assets/hero.jpeg)

# Agent Co-op

### The person is not the message bus

**Agent Co-op and the case for coordinating AI agents through files**

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
![Version](https://img.shields.io/badge/version-0.3-blue)
![Pages](https://img.shields.io/badge/pages-25-lightgrey)

### 📄 [Download the white paper (PDF)](AGENT-COOP_WhitePaper_v0.3.pdf)

---

## What this is

A design paper on a file-based protocol for AI agents working together on one computer.

People who split work across more than one AI assistant end up carrying messages between them. Formatting breaks on the way. Answers arrive late, or in several pieces. Agent Co-op removes that copying. Agents on one computer read and write plain files in a shared folder, called the board. It adds no server and no process of its own, needs no account, and nothing listens on a network port except an optional local viewer. A message is one file, written once and never edited.

The argument is that moving messages is the easy part. The hard part is who is allowed to do what. Each project has one driver, the only agent that edits the project. Every other agent is a helper that answers the driver and never edits. A message is information, never an order. Only the person approves risky actions, and only the person changes who holds which role.

The board keeps a record and checks its rules. It does not, by itself, stop an agent from breaking them. Enforcement depends on each tool's permissions and on the operating system.

This paper does not claim the design is proven. There is one user, on one project. It does not report measured time saved. Features added in software version 0.2.0 are described as designed, not as shown to work. It does not claim the board prevents rule-breaking. It does not claim to replace network protocols for agents. It solves a narrower problem: agents on one computer, working for one person.

**Software:** [agent-coop](https://github.com/zlatko-lakisic/agent-coop) (Apache License 2.0)

---

## What the paper covers

| Section | Contents |
|---|---|
| **Executive summary** | The relay, the board, and the line between a record and enforcement |
| **1. The failure mode** | The person as the message bus between a reasoning agent and a coding agent |
| **2. What the fix had to do** | Requirements traced to the relay, including no added infrastructure |
| **3. Why not an existing approach** | MCP, A2A, orchestration frameworks, and the blackboard |
| **4. How the board works** | One file per message, written once, answered by reference, marked handled |
| **5. Authority is the design** | One driver, helpers who do not talk to each other, and the cost of that rule |
| **6. What the person still does** | Copying is gone. The person is still the clock |
| **7. The approval gate** | Watching while present, and a separate branch for unattended runs |
| **8. Known considerations** | Policy versus enforcement, detection, known gaps, and how it could be tested |
| **9. Conclusion** | The rules make the work legible. The person still starts every agent |
| **Appendix A** | Protocol summary for builders |
| **Appendix B** | License and citation |

25 pages, 8 figures.

---

## Suggested citation

Lakisic, Z. (2026). *The person is not the message bus: Agent Co-op and the case for coordinating AI agents through files.* White paper, version 0.3.

---

## License

Licensed under [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) (CC BY 4.0).

You are free to share and adapt this material, including commercially, provided you give appropriate credit.

See [LICENSE](LICENSE) and [LICENSE.md](LICENSE.md).

The Agent Co-op software is separately licensed under the Apache License 2.0.

---

## Feedback

Corrections and disagreement are welcome, especially on the driver and helper split, the line between policy and enforcement, and what would count as evidence beyond one user. Open an issue or reach out directly.

**Zlatko Lakisic**
[Portfolio](https://zlatko-lakisic.github.io/zlatko-lakisic/) · [LinkedIn](https://www.linkedin.com/in/zlatko-lakisic/) · [Software](https://github.com/zlatko-lakisic/agent-coop)
