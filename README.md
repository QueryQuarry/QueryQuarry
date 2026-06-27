# QueryQuarry

**The double-blind escrow marketplace for talent.** Where recruiters discover talent — not resumes.

QueryQuarry flips hiring around: instead of candidates blasting applications into the void, they upload a resume once and a structured, consent-based profile joins a private talent graph. Recruiters' AI assistants query that graph directly over [MCP](https://modelcontextprotocol.io) — searching, evaluating, and reaching out — while identities stay sealed on both sides until a candidate chooses to connect. No applications, no scraping, no ghosting. Everyone in the corpus chose to be there.

## How the MCP works (for developers)

QueryQuarry is, at its core, an **MCP server** — the recruiter's AI is the intelligence; we're the corpus.

- A recruiter connects QueryQuarry to their AI client (Claude, etc.) via **OAuth** or an API key.
- The AI calls tools to **search** the talent graph, **evaluate** a candidate in depth (anonymously — no name, contact, employer names, or dates), and **request contact**.
- Reaching out is a deliberate, metered, consent-gated action: the candidate is notified and decides whether to respond. Identity and contact are released only on acceptance — the "double-blind escrow."
- Every match is logged so candidates can see how they were found, and contact runs through a per-pair claim code rather than exposed inboxes.

The result: a recruiter can open their AI, ask for "a senior React engineer open to remote, authorized to work in the US," and get real, anonymous, verified candidate cards back in seconds — without a single application being filed.

📚 **MCP documentation:** [queryquarry.com/docs/mcp](https://queryquarry.com/docs/mcp)

## Get started

- **Recruiters — connect QueryQuarry to your AI:** [queryquarry.com/recruiter/docs](https://queryquarry.com/recruiter/docs)
- **Candidates — upload your resume:** [queryquarry.com/upload](https://queryquarry.com/upload)
- **Home:** [queryquarry.com](https://queryquarry.com)

## Tech stack

- **Next.js** (App Router) + **React** — web app and API
- **Supabase** (Postgres + RLS) — data layer with row- and column-level access control
- **Stytch** — OAuth / Connected Apps for recruiter AI authentication
- **MCP** — the recruiter-facing AI interface to the talent graph

## Contact

[hello@queryquarry.com](mailto:hello@queryquarry.com)
