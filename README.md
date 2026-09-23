# Cherri skill

A Claude Code / Claude skill for writing [Cherri](https://github.com/electrikmilk/cherri) code - the DSL that compiles to Apple Shortcuts. It gives an agent a quick syntax reference and a list of known gotchas, then has it locate, verify freshness of, and read the user's own local clone of the [cherrilang.org docs](https://github.com/electrikmilk/cherrilang.org) for anything more specific.

This skill is for *authoring* `.cherri` files, not for contributing to the Cherri compiler itself.

## Install

Clone this repo into wherever your agent looks for skills, for example:

```console
git clone https://github.com/electrikmilk/cherri-skill ~/.claude/skills/cherri
```

## Requirements

- Nothing strictly required to use the syntax reference and gotchas in `SKILL.md`.
- A local clone of https://github.com/electrikmilk/cherrilang.org lets the agent look up anything beyond the basics (specific actions, standard library behavior, the package manager, etc.). The skill will ask where it's cloned the first time it needs it.
- The `cherri` CLI on `PATH` lets the agent verify action signatures and actually compile the code it writes.

## Links

- Language and compiler: https://github.com/electrikmilk/cherri
- Docs: https://cherrilang.org
- Playground: https://playground.cherrilang.org
