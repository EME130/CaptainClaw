Jot down learnings and information from the current session into the contributor's LootChest brain (Obsidian vault), organized naturally by topic.

## Instructions

1. Identify the contributor name from $ARGUMENTS. If not provided, ask for it. The contributor's vault lives at `LootChest/<NAME>/`.

2. If `LootChest/<NAME>/` doesn't exist, create the directory.

3. Scan the existing vault structure to understand what brain notes already exist:
   - Read all `.md` files in `LootChest/<NAME>/` (excluding `Todos.md`)
   - Understand the current topic groupings

4. Gather the key information from the current conversation session:
   - Decisions made and their rationale
   - Research findings (what works, what doesn't, and why)
   - Technical discoveries about the codebase
   - Tool/library evaluations
   - Architecture or design insights

5. Organize the information into the brain naturally:
   - **Group by topic** - don't just dump everything into one file. Use separate notes for distinct topics (e.g., `Audio.md`, `Build System.md`, `Proprietary Assets.md`)
   - **Grow existing notes** - if a relevant note already exists, append to it rather than creating a new one
   - **Create new notes** when the topic doesn't fit any existing note
   - **Link between notes** using Obsidian wikilinks `[[Note Name]]`
   - **Link to todos** where relevant: `[[Todos]]`

6. Formatting guidelines:
   - Use clear headings (`##`) for sections within a note
   - Use bullet points for facts and findings
   - Use `>` blockquotes for important warnings or decisions
   - Use inline code for file paths and commands
   - Add a `---` separator and date stamp (`*Added: YYYY-MM-DD*`) when appending to existing notes
   - Keep it concise but complete enough to be useful months later

7. Example brain note structure:
```markdown
# Audio

## Title Music
- Original `ClawLauncher/Resources/TITLE.wav` is proprietary - needs replacement
- Plan: AI-generate a new track inspired by "Computer Love"
- MusicGen (Meta) is best option - open source, supports audio conditioning
- NVIDIA Personaplex evaluated and ruled out (conversational AI, not music gen)

## Sound Effects
- ...

See also: [[Todos]], [[Proprietary Assets]]
```

8. Show the contributor a summary of what was added/updated and where.
