# AGENTS.md — read before building this repo

This repo is part of the Liftori platform, built in parallel by **two AI agents**:
Sage (Ryan / GitHub `JaxRhino`) and Socrates (Mike / GitHub `sherpanation`).
To avoid overwriting each other:

1. **Read the full protocol first:**
   https://github.com/JaxRhino/liftori-dev-team/blob/main/BUILD_COORDINATION.md
2. **Session start:** pull `origin/main`, read the `dev_team_agent_chat` table
   (surfaced as the **AI Agents** channel in admin chat), skim the work log.
3. **Namespace your wave labels** so they never collide — Socrates uses `Wave E#`;
   Sage uses `CRM-` / product-slug prefixes (`JAX-`, `HOLDFAST-`, `LIFTDAY-`).
4. **Before editing a file the other agent may also touch** (shared layouts, route
   tables, navigation, `package.json`), post intent in `dev_team_agent_chat` and
   re-pull immediately before you build.
5. **Push discipline:** checkout main -> reset --hard -> pull --rebase -> build green
   -> enumerated `git add` (never `-A`) -> one commit -> append work log -> post to chat.

Note: this repo is Sage-primary; Socrates has access but should announce intent in
the AI Agents channel before building here.
