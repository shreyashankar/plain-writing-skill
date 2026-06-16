# Plain writing skill

This skill makes an AI agent write in a plain style. The full rules are in
`SKILL.md`.

The rules are plain text, so any agent can use them.

The skill also checks its own writing. It removes anything that does not add
something, and it writes an HTML file that shows what it changed.

## What is in here

- `SKILL.md`: the skill, with the rules and the steps.
- `assets/revision_template.html`: the template for the change view. The skill
  fills it in with the edits it made.

## How to use it

`SKILL.md` is a plain markdown file with the rules. Any agent that can read a
file can follow it. The simplest way is to give `SKILL.md` to the agent as
instructions, in a rules file or the system prompt.

Some tools have a set place for skills:

- Claude Code reads skills from `~/.claude/skills`. Clone the repo into a folder
  named `plain-writing`:

```
git clone https://github.com/shreyashankar/plain-writing-skill ~/.claude/skills/plain-writing
```

- Other agents, e.g., Codex or pi, can use the rules too. Paste the rules from
  `SKILL.md` into whatever instructions that agent reads.

Then ask the agent to write or revise some text. It applies the rules on its
own.

When the agent removes or rewrites something, it writes an HTML file to `/tmp`.
The file has three tabs:

- First draft
- Second draft
- Diff

In the Diff tab the removed text is red and the rewritten text is green. The
reason for each change appears when you hover the colored text.

![The Diff tab, with removed text in red and rewritten text in green](docs/diff-view.png)
