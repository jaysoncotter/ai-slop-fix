# ai-slop-fix

A skill for finding and rewriting AI slop in professional writing. Works with any assistant that reads skills, custom instructions, or a system prompt.

Slop is coverage without decisions: writing that touches every part of the request while committing to nothing a person who knew the subject would have committed to. It usually isn't wrong. It's unfalsifiable.

## What's in it

A flat catalog of 25 named tells, alphabetical, no hierarchy. Each one shows the tell, fixes it, and says when the same construction is fine. You find the tell and apply the fix. There's nothing to classify first.

A few of them: the bolted-on benefit, elevating negation, the floating pronoun, the hedge stack, metronome punctuation, the runway, the stripped condition, two-sided nothing.

Then two shorter sections. One lists eleven things that look like tells and aren't, because over-flagging costs as much as under-flagging. The other covers what only shows up when you read a whole document: the closing line that was added to sound conclusive, and claims that appear twice, once with evidence and once as a maxim.

## Example

> ✗ "The maintenance log isn't just a record — it's the foundation of a safer fleet."
>
> ✓ "The maintenance log shows which vehicles are overdue for inspection."

> ✗ "The dashboard centralizes shift data, ensuring a seamless manager experience."
>
> ✓ "The dashboard pulls shift data from three systems, which cut schedule-building time from 40 minutes to 15."

## Use it

The skill is one Markdown file, `ai-slop-fix/SKILL.md`, with YAML frontmatter on top. Pick whichever of these fits your setup:

- **As a skill.** Copy the `ai-slop-fix/` folder into your assistant's skills directory. For tools that load skills from disk, that is usually `~/.claude/skills/` globally or `.claude/skills/` inside a project.
- **As project instructions.** Paste the file into custom instructions, a project knowledge base, or a `CLAUDE.md` or `AGENTS.md` at your repo root.
- **As a system prompt.** Prepend it to a system or developer message for a drafting or editing agent.
- **By hand.** Read it. The catalog works without a model in the loop.

The frontmatter (`name`, `description`) is what tells a skill-aware tool when to load the file. Strip it if you're pasting the body somewhere that doesn't want it.

It applies to memos, decks, reports, emails, and docs, whether you're drafting, editing, or reviewing.

## License

MIT
