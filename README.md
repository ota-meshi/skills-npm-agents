# Reproduce Repo

In this repository, after `npm install`, if you run the following command, an error will occur.

```sh
npx skills-npm --agents=github-copilot
```

Output:

```txt
┌  skills-npm@0.0.3
│
◇  Scanned 569 packages, found 1 skill
│
●  Discovered skills:
  ● slidev from @slidev/cli
    Create and present web-based slides for developers using Markdown, Vue components, code highlighting, animations, and interactive features. Use when building technical presentations, conference talks, or teaching materials.
file:///workspaces/skills-npm-agents/node_modules/skills-npm/dist/cli.mjs:199
        const message = `Target agents: ${c.cyan(targetAgents.join(", "))}`;
                                                              ^

TypeError: targetAgents.join is not a function
    at getTargetAgents (file:///workspaces/skills-npm-agents/node_modules/skills-npm/dist/cli.mjs:199:56)
    at CAC.<anonymous> (file:///workspaces/skills-npm-agents/node_modules/skills-npm/dist/cli.mjs:112:30)
```