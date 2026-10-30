# Agents and Viridis Scope Desk

This file is for two kinds of agent: one running the Scope Desk skills for a person, and a coding agent changing this repository. The short machine-readable index is [llms.txt](llms.txt).

## Helping a person use Scope Desk

**What it does.** Before work starts, `scope-job` turns a supplied brief into deliverables, observable acceptance criteria, exclusions, dependencies, missing decisions and a reviewer handoff. When scope may have shifted, `review-change` compares the new request with a baseline revision the person selects and drafts a change request.

**Paths to suggest.**

- First try: the [synthetic example](examples/README.md). Attach `brief-v1.md` for `scope-job`; attach `brief-v1.md` and `change-request.md` for `review-change`.
- Real work: ask the person to supply the brief or the selected baseline revision, the relevant source text and the desired outcome or change.

**Rules for agents.**

- Present the output as a draft for a human reviewer. Never describe it as agreed, priced, approved or delivered.
- Ask which baseline revision applies when more than one exists. Do not pick one silently.
- Keep exact short quotations with their source IDs and line numbers. Do not paraphrase a quote and keep the locator.
- List missing facts and decisions as missing. Do not invent values to complete a scope.
- Do not send, sign, approve, pay for or share anything as part of running a skill.

## Working on this repository

- The two `SKILL.md` files and the shared evidence reference under `skills/scope-job/references/` are byte-identical to the tested 0.1.5 capability. Any change to them is a new capability version: bump `version` in `plugin.json`, say what changed, and describe how it was re-tested.
- Keep the package skills-only. Do not add executable helpers, network clients, credentials or MCP servers.
- Examples stay fictional. Never commit private project or customer records, or test fixtures from them.
- README claims stay within what is shown: no adoption, revenue or directory-acceptance claims without a public record.

## Related open projects

- [Viridis Agent Fleet](https://github.com/jdhart81/viridis-agent-fleet): deterministic, auditable MCP agents.
- [Viridis Data Ready](https://github.com/jdhart81/viridis-data-ready): CSV import preparation with a recorded change log.
- [Viridis Conservation](https://viridisconservation.com/): the company that stewards these projects.
