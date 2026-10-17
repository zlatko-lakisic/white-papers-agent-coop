![Agent Co-op](assets/hero.jpeg)

# Agent Co-op

### The Person Is Not the Message Bus

**Agent Co-op and the case for coordinating AI agents through files**

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
![Version](https://img.shields.io/badge/version-0.2-blue)
![Pages](https://img.shields.io/badge/pages-23-lightgrey)

### 📄 [Download the white paper (PDF)](AGENT-COOP_WhitePaper_v0.2.pdf)

---

## What this is

A design paper on a file-based protocol for AI agents working together on one computer.

People who split work across more than one AI assistant end up carrying messages between them. Formatting breaks on the way. Answers arrive late, in pieces, or out of order. Agent Co-op removes that relay. Agents on one computer read and write plain files in a shared folder, called the board. There is no server, no account, and no network port. A message is one file, written once and never edited.

The argument is that moving messages is the easy part. The hard part is who is allowed to do what. Each project has one driver, the only agent that edits the project. Every other agent is a helper that answers the driver and never edits. A message is information, never an order. Only the person approves risky actions, and only the person changes who holds which role.

This paper does not claim the design is proven. There is one user, on one project. It does not report measured time saved. Features added in software version 0.2.0 are described as designed, not as shown to work. It does not claim to replace network protocols for agents. It solves a narrower problem: agents on one computer, working for one person.

**Software:** [agent-coop](https://github.com/zlatko-lakisic/agent-coop) (Apache License 2.0)

---

## What the paper covers

| Section | Contents |
|---|---|
| **Executive summary** | The relay, the board, and the authority rules |
| **1. The failure mode** | The person as the message bus between a reasoning agent and a coding agent |
| **2. What the fix had to do** | Requirements traced back to the relay and to tools already in use |
| **3. Why not an existing protocol** | MCP, A2A, and the blackboard architecture |
| **4. How the board works** | One file per message, written once, answered by reference, marked handled |
| **5. Authority is the design** | One driver, helpers who answer, messages that are not orders |
| **6. What the person still does** | Copying is gone. Starting agents, direction, and judgment remain |
| **7. The approval gate** | Scheduled work lands on a branch the driver cannot push |
| **8. Known considerations** | One computer, detection rather than prevention, one user |
| **9. Conclusion** | Files move the messages. The rules decide who may write them |
| **Appendix A** | Protocol summary for builders |
| **Appendix B** | License and citation |

23 pages, 8 figures.

---

## Suggested citation

Lakisic, Z. (2026). *The Person Is Not the Message Bus: Agent Co-op and the Case for Coordinating AI Agents Through Files.* White paper, version 0.2.

---

## License

Licensed under [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) (CC BY 4.0).

You are free to share and adapt this material, including commercially, provided you give appropriate credit.

See [LICENSE](LICENSE) and [LICENSE.md](LICENSE.md).

The Agent Co-op software is separately licensed under the Apache License 2.0.

---

## Feedback

Corrections and disagreement are welcome, especially on the driver and helper split, the claim that authority matters more than transport, and what would count as evidence beyond one user. Open an issue or reach out directly.

**Zlatko Lakisic**
[Portfolio](https://zlatko-lakisic.github.io/zlatko-lakisic/) · [LinkedIn](https://www.linkedin.com/in/zlatko-lakisic/) · [Software](https://github.com/zlatko-lakisic/agent-coop)
